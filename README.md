# Boreas Environment Generator

A tool to provision and manage Boreas Environments.

## Prerequisites

1. Install latest [Node LTS](https://nodejs.org).
2. `npm install -g yo`
3. Clone this repo: `git clone git@github.com:logrhythm/generator-boreas-env.git && cd generator-boreas-env`
4. Install dependencies: `npm install`
5. Run `npm link` to create a symlink in the global folder so `yo` can use this module.
6. Github personal access token with SSO enabled for the Logrhythm org: https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token

**Other dependencies:**

Versions are currently defined in generator-tools.yaml
- terraform
- terragrunt
- kops
- kubectl
- kubeseal cli
- jq
- aws-cli, follow the CLI and Okta setup [here](https://confluence.logrhythm.com/display/NGP/AWS+CLI+usage)
- [aws-iam-authenticator](https://docs.aws.amazon.com/eks/latest/userguide/install-aws-iam-authenticator.html)
- [AWS SessionManagerPlugin (SSM)](https://confluence.logrhythm.com/display/NGP/AWS+Session+Manager)

## How to use

1. Create a new directory which will be use for storing environment configuration
2. _In that directory_, run `yo boreas-env` and follow the instruction, the generator will:
  - Prompt for some shared configurations:
    -  Namespace
    -  Environment
    -  GitOps URL
  - Provision some share configurations for all vpcs and clusters
3. Run `yo boreas-env:cluster` and follow the instruction, the generator will:
  - Ask for the info of the vpc housing the cluster:
    - VPC Name
    - VPC Cidr
    - Is this VPC for Shared Services?
  - Ask for the info of the cluster:
    - Cluster Name
    - Workloads to deploy to this cluster
    - Version of Kops Configuration Template
  - Ask for some other workloads' configuration that is needed for bootstrapping the cluster
  - Generate Terraform code for VPC, Subnets, and other resources for Kops then execute these terraform code
  - Generate Kops configuration then provision the cluster using Kops
  - Generate Kubernetes workloads' descriptors
  - Bootstrap the cluster:
    - Config the AWS IAM Authenticator (so that we can authenticate to kubeapi server using AWS IAM User)
    - Create a custom kubeconfig file to use AWS IAM instead of the generated username/password from Kops
    - Install SealedSecrets
    - Generate ArgoCD's SealedSecrets (to store Github token)
    - If Atlantis is selected
      - Generate webhook token for Atlantis
      - Generate Atlantis's SealedSecrets (to store Github token and webhook token)
    - Request user to push configuration to GitOps repo
    - Deploy ArgoCD
    - Deploy the "app of app" of ArgoCD
4. To update K8s workloads' descriptors to what are currently defined in the current generator version:

    ```zsh
    yo boreas-env:cluster-workload-update --vpc VPC_DIR_NAME --cluster CLUSTER_SHORT_NAME [--reconfigure-workload]
    ```
5. To update existing cluster kops to a specific config version:

    ```zsh
    yo boreas-env:cluster-kops-update --vpc VPC_DIR_NAME --cluster CLUSTER_SHORT_NAME [--reconfigure-kops]
    ```

To see available options for a generator's command, add `--help` option when calling the generator. For example:

```zsh
yo boreas-env --help
yo boreas-env:cluster --help
yo boreas-env:cluster-workload-update --help
yo boreas-env:cluster-kops-update --help
yo boreas-env:cluster-destroy --help
```

## Guides

### Destroy a cluster

Run the following command to destroy a cluster (replace `VPC_DIR_NAME` and `CLUSTER_SHORT_NAME` with correct values)

```bash
yo boreas-env:cluster-destroy --vpc VPC_DIR_NAME --cluster CLUSTER_SHORT_NAME
```

You can add more options to the commands to customize the process like:

- `--skip-confirm` Auto approves all Terraform plans and confirmations if possible
- `--skip-sealedsecrets` Skip backing up Sealed Secret Master keys

To see all available options, please run `yo boreas-env:cluster-destroy --help`

### Connect to a cluster from your local computer

```bash
yo boreas-env:cluster-connect
```

To see all available options, please run `yo boreas-env:cluster-connect --help`

## Other commands

### yo boreas-env:cluster-kops-update

To update kops config, Kubernetes versions or execute any change to SSH keys, a kops update is necessary.

If Kubernetes version is updated, or SSH keys were mutated, then an additional rolling-update is necessary. The below procedure will execute it if needed.

1. Install appropriate kops version, if upgrading to a new minor release of Kubernetes (kops major.minor should correspond to Kubernetes major.minor)
2. run `yo boreas-env:cluster-kops-update`

cluster-kops-update manages the entire kops update lifecycle automatically. It determines if a rolling update is necessary and, if so, orchestrates that process and handles tainting nodes whose pods won't evict. Internally, it also handles the concerns of cluster connection and will automatically reconnect to a new master should the currently connected master get rolled. The automated process can take a while - anywhere from 20-30 minutes currently, so be patient. You should see similar output as this upon successful completion:

```
[Generator] Kops Rolling Update Complete

[Generator] Kops command finished...
The following node:pod list shows the pods that resulted in manual node taints:
        ip-10-36-87-35.us-west-2.compute.internal:boreas-search-indexing-svc-pg-0
        ip-10-36-87-35.us-west-2.compute.internal:boreas-unleash-pg-1
        ip-10-36-87-35.us-west-2.compute.internal:boreas-keycloak-pg-1
        ip-10-36-87-35.us-west-2.compute.internal:boreas-search-indexing-svc-es-data-2
        ip-10-36-80-135.us-west-2.compute.internal:boreas-search-indexing-svc-es-data-1
        ip-10-36-103-226.us-west-2.compute.internal:boreas-content-management-svc-pg-1
        ip-10-36-103-226.us-west-2.compute.internal:boreas-access-control-svc-pg-0
        ip-10-36-103-226.us-west-2.compute.internal:kube-dns-64f86fb8dd-vrn2s
        ip-10-36-103-226.us-west-2.compute.internal:boreas-notification-svc-pg-1
        ip-10-36-103-226.us-west-2.compute.internal:boreas-audit-svc-pg-1
        ip-10-36-103-226.us-west-2.compute.internal:istio-telemetry-74bcdf74d5-8xhb6
```

## Utils

### Update all default workloads' configs
The `defaultWorkloadConfig` defined for workloads in `generators/cluster/workloads.js` can be far out of date with what is in `boreas-env-development`. As a result, the new environment bootstrapped with the generator might not work as expected. There is a script to help updating all `defaultWorkloadConfig` in the generator:

```zsh
npm run update-workload-configs-from-dev
```

Note: this command will mutate `generators/cluster/workloads.js`.

## Troubleshooting

When you are having problem running the command like an error make your script stop but some action cannot be done twice. You can add options to the command to skip certain actions/steps like `--skip-kops`, etc.

If running into any issue add -v before -tt at line 165 in 'generators/aws.js' to check the verbose. 
   looks like this "-v -tt -N -L"

To check the version of the generator, use "npm ls -g --depth=0  generator-boreas-env"

## Contributing
Please follow below guideline when contributing to this project
- Conventional commit: https://www.conventionalcommits.org/en/v1.0.0/

## TODO:
- Add Atlantis configuration (dynamically generated by the generator)
- Add tooling container that includes necessary versions of kops, terraform, terragrunt, kubectl, etc.
- Secure pomerium and keycloak credentials
- Secure LogRhythm Operator's slack webhook token
