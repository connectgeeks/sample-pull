## [21.1.2](https://github.com/logrhythm/generator-boreas-env/compare/v21.1.1...v21.1.2) (2021-04-30)


### Bug Fixes

* adding scheduling-svc as dependency ([83c492a](https://github.com/logrhythm/generator-boreas-env/commit/83c492a2442ffaea479b6d0d4f968c14edf9db85))
* removing extra unneeded env variables since lr-operator can trigger rolling update when cm changes ([8bfeb34](https://github.com/logrhythm/generator-boreas-env/commit/8bfeb34fa71a80ab244442efd75a2f2679e26f31))

## [21.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v21.1.0...v21.1.1) (2021-04-28)


### Bug Fixes

* update default workload config ([bddd110](https://github.com/logrhythm/generator-boreas-env/commit/bddd110429b8c2ba59c8d2e98aadc996ddfbbc83))

# [21.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v21.0.0...v21.1.0) (2021-04-28)


### Features

* **terraform:** update infra/kops module to speed up environment teardown ([141d019](https://github.com/logrhythm/generator-boreas-env/commit/141d019de76e32a5773c3d499f5d8e8e8cf0d7d1))

# [21.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v20.6.0...v21.0.0) (2021-04-28)


* feat!: update LR Operator manifests ([d49d9fc](https://github.com/logrhythm/generator-boreas-env/commit/d49d9fc9bb19b43baa1ae41ccd7d58b3d7019b2e))


### BREAKING CHANGES

* need to update logrhythm-operator docker image to v0.29.0

# [20.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v20.5.1...v20.6.0) (2021-04-27)


### Features

* modify default image to newest for lr-operator ([3ed7a76](https://github.com/logrhythm/generator-boreas-env/commit/3ed7a76583cd06ec640f7b5f2527172e67f36ef6))

## [20.5.1](https://github.com/logrhythm/generator-boreas-env/compare/v20.5.0...v20.5.1) (2021-04-23)


### Bug Fixes

* use updated boreas-kubernetes version of kafka-system to remove noisy alert rule ([9e5352c](https://github.com/logrhythm/generator-boreas-env/commit/9e5352cfb6089ec4a99fe4eceef18b6120d175d3))

# [20.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v20.4.0...v20.5.0) (2021-04-22)


### Features

* upgrade generator to include new versions of boreas-kubernetes for kafka workloads ([1f209b7](https://github.com/logrhythm/generator-boreas-env/commit/1f209b791e3ef8306b3b1adc6c30a92fa9d9d148))

# [20.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v20.3.0...v20.4.0) (2021-04-20)


### Features

* Update Pomerium to 0.13.6 ([df92d70](https://github.com/logrhythm/generator-boreas-env/commit/df92d70385f78c62b2fb1ae0dce3c912035db35a))

# [20.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v20.2.0...v20.3.0) (2021-04-20)


### Bug Fixes

* Bump CMS request CPU to 500m to be consistent for now ([1491a25](https://github.com/logrhythm/generator-boreas-env/commit/1491a251778b54a37d5041a7e3902ccb19e581ba))
* configure number of threads for kafka streams to ensure there is one thread per partition in the topic ([2b22a79](https://github.com/logrhythm/generator-boreas-env/commit/2b22a79cc65d15f546d6e837a0f60f7166d8a351))


### Features

* Hard-set replica count, increase CPU/RAM, and increase session timeout and heartbeat interval ([d494199](https://github.com/logrhythm/generator-boreas-env/commit/d4941993e604c5bd3476f876e88cebf9bac60740))
* Update HPA and resource config for content-mgmt, signal-ident, signal-norm, and topology-svc ([66ad8c8](https://github.com/logrhythm/generator-boreas-env/commit/66ad8c8735bb8b38523f8d2b73501e660ffa5cfa))

# [20.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v20.1.0...v20.2.0) (2021-04-16)


### Features

* additional capabilities for cdo cache ([4c60d48](https://github.com/logrhythm/generator-boreas-env/commit/4c60d48957b13403834ebad383fb6dea01121d2b))
* additional cdo cache capabilities ([0b494ce](https://github.com/logrhythm/generator-boreas-env/commit/0b494ce62a85741b392433fc9e7e2f63a306fce8))

# [20.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v20.0.2...v20.1.0) (2021-04-15)


### Features

* add PROCESS_SIGNAL capability to azure-collector-svc ([9f091b7](https://github.com/logrhythm/generator-boreas-env/commit/9f091b70c4373e47956928c17ca669adacb03fd4))

## [20.0.2](https://github.com/logrhythm/generator-boreas-env/compare/v20.0.1...v20.0.2) (2021-04-14)


### Bug Fixes

* update default workload config ([0eedc52](https://github.com/logrhythm/generator-boreas-env/commit/0eedc527cf04ae118c9a05bd6981797668083c53))

## [20.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v20.0.0...v20.0.1) (2021-04-14)


### Bug Fixes

* correct argocd version's reference and add reconfigure-workload to cluster-workload-update-all ([d5fb418](https://github.com/logrhythm/generator-boreas-env/commit/d5fb4184258d0b12472bf6371792d709041b7d79))

# [20.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v19.4.0...v20.0.0) (2021-04-14)


### Bug Fixes

* update google-flink-operator version's reference ([813931f](https://github.com/logrhythm/generator-boreas-env/commit/813931f391efc2e4f227d9079b59302d4d18b35c))


* feat!: add Google Flink Operator, streaming-analytics-app, and remove streaming-aggregation-app ([2d3d3d9](https://github.com/logrhythm/generator-boreas-env/commit/2d3d3d99cce465aa9f7c514ca91b5d1bb4cb7283))


### BREAKING CHANGES

* streaming-aggregation-app is removed, you will need to update your cluster workload with `--reconfigure-workload` option so the generator can remove streaming-aggration-app correctly

# [19.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v19.3.1...v19.4.0) (2021-04-12)


### Features

* **pomerium:** Update Pomerium ([66a8384](https://github.com/logrhythm/generator-boreas-env/commit/66a83844ba7efa3ee768f5678dd44ac27d3506f8))

## [19.3.1](https://github.com/logrhythm/generator-boreas-env/compare/v19.3.0...v19.3.1) (2021-04-10)


### Bug Fixes

* update default workload config ([b488e9a](https://github.com/logrhythm/generator-boreas-env/commit/b488e9a5c5546c95c55bf8c66f73a12067db7c03))

# [19.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v19.2.0...v19.3.0) (2021-04-09)


### Features

* **keycloak:** Update to boreas-keycloak 8.4.0, upgrading Keycloak to 12.0.4 ([331eaa2](https://github.com/logrhythm/generator-boreas-env/commit/331eaa255c392caaf9bb6b8e56a01773fabc25e2))

# [19.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v19.1.0...v19.2.0) (2021-04-08)


### Features

* Reorder waves, moving Jaeger and Prometheus to be deployed with all other observability tools ([e0ac3cb](https://github.com/logrhythm/generator-boreas-env/commit/e0ac3cb2bf4c1e73f01e514d4d52ac4f4053ff84))

# [19.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v19.0.0...v19.1.0) (2021-04-08)


### Features

* upgrade strimzi kafka to v0.22.1 ([8083131](https://github.com/logrhythm/generator-boreas-env/commit/8083131a71afe5c9c54c62cdf3dc88f0328a00ed))

# [19.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.13.2...v19.0.0) (2021-04-07)


### Features

* Upgrade prometheus-operator boreas-kubernetes to v8.2.0 ([06de981](https://github.com/logrhythm/generator-boreas-env/commit/06de98145aa69e9b0416b700db69dbcd98be9249))
* Upgrade Sonarqube boreas-kubernetes to v8.3.0 ([a5b7dee](https://github.com/logrhythm/generator-boreas-env/commit/a5b7dee4f78022bf0b7f04e50297e2a1a471abb4))


### BREAKING CHANGES

* New CRDs must be deployed manually and prometheus-system argocd application deleted
`find prometheus-operator/upstream/kube-prometheus-stack/crds -type f -exec kubectl apply -f {} \;`

## [18.13.2](https://github.com/logrhythm/generator-boreas-env/compare/v18.13.1...v18.13.2) (2021-04-07)


### Bug Fixes

* update default logrhythm-operator version ([3fc9b46](https://github.com/logrhythm/generator-boreas-env/commit/3fc9b46f5c3089550b23492051b9b38216a5e0da))

## [18.13.1](https://github.com/logrhythm/generator-boreas-env/compare/v18.13.0...v18.13.1) (2021-04-07)


### Bug Fixes

* update default workload config ([0e85435](https://github.com/logrhythm/generator-boreas-env/commit/0e85435ef1615552abf1592f1dfacc7f33ba53f9))

# [18.13.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.12.0...v18.13.0) (2021-04-06)


### Features

* update the component dependies based on PR[#2522](https://github.com/logrhythm/generator-boreas-env/issues/2522) ([c2f49ad](https://github.com/logrhythm/generator-boreas-env/commit/c2f49ad31eb05da745221b15ca17faf8cdd2cef3))

# [18.12.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.11.1...v18.12.0) (2021-04-05)


### Features

* remove db from audit-svc ([80aa702](https://github.com/logrhythm/generator-boreas-env/commit/80aa702b1de6c98c28ced9cebd3a3dde053eda70))

## [18.11.1](https://github.com/logrhythm/generator-boreas-env/compare/v18.11.0...v18.11.1) (2021-04-05)


### Bug Fixes

* update default workload config ([c125f35](https://github.com/logrhythm/generator-boreas-env/commit/c125f353bad1d9f0b1333cabfb014ad870c5da16))

# [18.11.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.10.0...v18.11.0) (2021-04-02)


### Features

* deploy ms-graph-collector-svc ([e14ce1e](https://github.com/logrhythm/generator-boreas-env/commit/e14ce1ea627483e5c3372f12eb1e7f45069a6077))

# [18.10.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.9.0...v18.10.0) (2021-04-01)


### Features

* update audit-svc properties ([903385c](https://github.com/logrhythm/generator-boreas-env/commit/903385c52a2bb9e7410d2be754a40366ad15db55))

# [18.9.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.8.0...v18.9.0) (2021-04-01)


### Features

* add capability to topology-svc ([c470e65](https://github.com/logrhythm/generator-boreas-env/commit/c470e658bf5f4a9c2562dc23cfa1e7db832acdb5))

# [18.8.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.7.0...v18.8.0) (2021-04-01)


### Features

* add sip-management-svc to swagger ([df53358](https://github.com/logrhythm/generator-boreas-env/commit/df53358159c73307777a162da753a52ec5d616b2))

# [18.7.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.6.2...v18.7.0) (2021-03-30)


### Bug Fixes

* updating the component dependencies ([8dde1e9](https://github.com/logrhythm/generator-boreas-env/commit/8dde1e91fafb191dd7342650f507849fa5e87f08))


### Features

* adding sip-management-svc workloads ([cee6aec](https://github.com/logrhythm/generator-boreas-env/commit/cee6aec8b64d331517194db2242538ddcd2a1091))

## [18.6.2](https://github.com/logrhythm/generator-boreas-env/compare/v18.6.1...v18.6.2) (2021-03-29)


### Bug Fixes

* update default workload config ([4bb4b75](https://github.com/logrhythm/generator-boreas-env/commit/4bb4b75e96ebdc9631a18e24365569760b7e0332))

## [18.6.1](https://github.com/logrhythm/generator-boreas-env/compare/v18.6.0...v18.6.1) (2021-03-29)


### Bug Fixes

* Topology and scheduling svc both use a single property as the base URL to call many services via REST ([4481c6f](https://github.com/logrhythm/generator-boreas-env/commit/4481c6f5705708a66bb522bf98988443dc680ae4))

# [18.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.5.0...v18.6.0) (2021-03-29)


### Features

* Override properties for cluster-internal REST calls in topology and scheduling-svc ([244dfc2](https://github.com/logrhythm/generator-boreas-env/commit/244dfc2e5445d2680575fed475d993cfd0785d3c))

# [18.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.4.0...v18.5.0) (2021-03-25)


### Features

* update the app properties of search-indexing-svc ([ed8b684](https://github.com/logrhythm/generator-boreas-env/commit/ed8b68439043427d384e18f7510941f0aeb8cd7c))

# [18.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.3.0...v18.4.0) (2021-03-24)


### Features

* add capability to notification-svc ([eb95b5f](https://github.com/logrhythm/generator-boreas-env/commit/eb95b5f5ccaaa7294b793ff97c2af6e88d6b656c))

# [18.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.2.0...v18.3.0) (2021-03-22)


### Features

* add capability to topology-svc ([b29f46d](https://github.com/logrhythm/generator-boreas-env/commit/b29f46df121fe174acc9792befcef8afb0f43df9))

# [18.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.1.0...v18.2.0) (2021-03-19)


### Features

* Incorporate subnet infra module updates to reduce config duplication ([2969c28](https://github.com/logrhythm/generator-boreas-env/commit/2969c280c3962e18577a0ff6dbf8a3f88e6cac5e))

# [18.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v18.0.1...v18.1.0) (2021-03-19)


### Features

* add new sub-generator to update workloads for all clusters at once ([dec63a1](https://github.com/logrhythm/generator-boreas-env/commit/dec63a14fb209bce1b76f720ce96314c293e9bcc))

## [18.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v18.0.0...v18.0.1) (2021-03-18)


### Bug Fixes

* correct kubernetes loki template ([5c40d14](https://github.com/logrhythm/generator-boreas-env/commit/5c40d1443260e0aa84ca8d76d9bac3de86911b65))

# [18.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.9.0...v18.0.0) (2021-03-18)


* feat(loki)!: fix Loki labels slow loading issue and upgrade Loki & Promtail ([2ae366b](https://github.com/logrhythm/generator-boreas-env/commit/2ae366be3c3848fce13f5e834242f252c4954bf8))


### BREAKING CHANGES

* need to delete loki statefulset from ArgoCD and re-sync loki ArgoCD app

# [17.9.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.8.0...v17.9.0) (2021-03-18)


### Features

* add cms to topology-svc ([a70918a](https://github.com/logrhythm/generator-boreas-env/commit/a70918a1aaf07b3902b3b3b747ae6068b3d9666d))

# [17.8.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.7.2...v17.8.0) (2021-03-16)


### Features

* **scheduling-svc:** update capabilities ([1e081d4](https://github.com/logrhythm/generator-boreas-env/commit/1e081d4f0fe55542b222b4051fdfe78686efb870))

## [17.7.2](https://github.com/logrhythm/generator-boreas-env/compare/v17.7.1...v17.7.2) (2021-03-12)


### Bug Fixes

* update default workload config ([0b0c1e5](https://github.com/logrhythm/generator-boreas-env/commit/0b0c1e5208f8d41bfd6d9dc409af07fc17ea87f2))

## [17.7.1](https://github.com/logrhythm/generator-boreas-env/compare/v17.7.0...v17.7.1) (2021-03-10)


### Bug Fixes

* update default workload config ([985e21f](https://github.com/logrhythm/generator-boreas-env/commit/985e21fbfc9109cd4b7a1e2599f9ca5cf5d0127b))

# [17.7.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.6.2...v17.7.0) (2021-03-10)


### Bug Fixes

* alphabetization ([847ba76](https://github.com/logrhythm/generator-boreas-env/commit/847ba76014a2d14b379b068e2fe54d0031e30eb3))


### Features

* deploy new prototype mfe ([25bae7f](https://github.com/logrhythm/generator-boreas-env/commit/25bae7f0743716a13a39fcb190c5eba980c8e768))

## [17.6.2](https://github.com/logrhythm/generator-boreas-env/compare/v17.6.1...v17.6.2) (2021-03-05)


### Bug Fixes

* increase resource limits for loki and promtail ([e1b033a](https://github.com/logrhythm/generator-boreas-env/commit/e1b033a9e6c8518a4c9789a4262446f92133db69))

## [17.6.1](https://github.com/logrhythm/generator-boreas-env/compare/v17.6.0...v17.6.1) (2021-03-03)


### Bug Fixes

* update default workload config ([8551625](https://github.com/logrhythm/generator-boreas-env/commit/85516253bb8f1512d789453d2b596313d1962809))

# [17.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.5.1...v17.6.0) (2021-03-03)


### Bug Fixes

* workloads.js order ([f3b8f26](https://github.com/logrhythm/generator-boreas-env/commit/f3b8f2683419c1df95741f52026343995134718a))


### Features

* deploy azure-collector-svc ([bd0a2d3](https://github.com/logrhythm/generator-boreas-env/commit/bd0a2d3939c60aff64fdf32f47a80b7c6c1e09a7))

## [17.5.1](https://github.com/logrhythm/generator-boreas-env/compare/v17.5.0...v17.5.1) (2021-03-02)


### Bug Fixes

* acs property ([86c50cb](https://github.com/logrhythm/generator-boreas-env/commit/86c50cbea2e7740131bd96815726a1e2b507dc5f))

# [17.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.4.0...v17.5.0) (2021-03-02)


### Features

* deploy new grid mfe ([90d9fe7](https://github.com/logrhythm/generator-boreas-env/commit/90d9fe703b11a2e99e2db95218425171adeee22b))

# [17.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.3.1...v17.4.0) (2021-03-02)


### Features

* update access-control-svc with new app.properties ([b7de664](https://github.com/logrhythm/generator-boreas-env/commit/b7de6640cbf93f0ec5b3ec2ff2d97ae926999d5d))

## [17.3.1](https://github.com/logrhythm/generator-boreas-env/compare/v17.3.0...v17.3.1) (2021-03-01)


### Bug Fixes

* update CMS's application.properties ([b9338d9](https://github.com/logrhythm/generator-boreas-env/commit/b9338d9abd7b1c3ed1e6271fbeae4701b2ff7ddf))

# [17.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.2.0...v17.3.0) (2021-02-25)


### Features

* updated keycloak runtime-config.js ([238a5c4](https://github.com/logrhythm/generator-boreas-env/commit/238a5c4a00c5dec0c57cd53f4a269b6fa938b8ad))

# [17.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.1.2...v17.2.0) (2021-02-25)


### Features

* add defaultTenantId to runtime-config.js ([bcea66e](https://github.com/logrhythm/generator-boreas-env/commit/bcea66e399fd0e638efbe23d48512f77f796553b))

## [17.1.2](https://github.com/logrhythm/generator-boreas-env/compare/v17.1.1...v17.1.2) (2021-02-23)


### Bug Fixes

* upgrade loki and infra/kops to enable lifecycle for loki bucket ([70d4795](https://github.com/logrhythm/generator-boreas-env/commit/70d47954d4ef9f4b66e4c62a9832d6196bf152af))

## [17.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v17.1.0...v17.1.1) (2021-02-23)


### Bug Fixes

* allowNonRestoredState enabled in streaming-aggregation-app ([5765975](https://github.com/logrhythm/generator-boreas-env/commit/57659752266f400bd0096bacf62f927366d4f65b))

# [17.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v17.0.0...v17.1.0) (2021-02-22)


### Features

* update version of logrhythm-system ([c0f42d6](https://github.com/logrhythm/generator-boreas-env/commit/c0f42d64f710139854b917089608cb55c85b1d1f))

# [17.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v16.3.1...v17.0.0) (2021-02-22)


### Bug Fixes

* point loki's resources to correct version ([e54d661](https://github.com/logrhythm/generator-boreas-env/commit/e54d661fa358eccb73e02fb0adf60edcef1aa1c0))


* feat!: upgrade Loki ([980106e](https://github.com/logrhythm/generator-boreas-env/commit/980106e886568cee51a956c96c58b528ce2f9573))


### BREAKING CHANGES

* Loki workload has been upgraded to a major version and migration is needed

Migration: delete Loki namespace and re-deploy Loki

## [16.3.1](https://github.com/logrhythm/generator-boreas-env/compare/v16.3.0...v16.3.1) (2021-02-22)


### Bug Fixes

* update capability for scheduling-svc ([723c551](https://github.com/logrhythm/generator-boreas-env/commit/723c551074a553b4023f47ffb07a0adc158782e1))

# [16.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v16.2.2...v16.3.0) (2021-02-18)


### Features

* use new svc-boreas-CICD user ([327cff0](https://github.com/logrhythm/generator-boreas-env/commit/327cff0e1844c6f52192e45da3601cac168ff3c4))

## [16.2.2](https://github.com/logrhythm/generator-boreas-env/compare/v16.2.1...v16.2.2) (2021-02-17)


### Bug Fixes

* add serviceAccount definition for scheduling-svc ([28d26fa](https://github.com/logrhythm/generator-boreas-env/commit/28d26fadf1d415a77ea0570546ffe46a66a683f1))

## [16.2.1](https://github.com/logrhythm/generator-boreas-env/compare/v16.2.0...v16.2.1) (2021-02-16)


### Bug Fixes

* change keycloak-oidc to Okta ([97b1d38](https://github.com/logrhythm/generator-boreas-env/commit/97b1d38bbc0f7a087fb8623c61e7948fcc152e0d))

# [16.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v16.1.0...v16.2.0) (2021-02-15)


### Features

* enable okta integration to boreas ([2dce0c5](https://github.com/logrhythm/generator-boreas-env/commit/2dce0c5b9a54b31981c41466f20799b219bf9a06))

# [16.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v16.0.3...v16.1.0) (2021-02-15)


### Features

* update Istio to 1.9.0 ([7f86367](https://github.com/logrhythm/generator-boreas-env/commit/7f86367a1c10e812b476f05be7b87551e1f3edb6))

## [16.0.3](https://github.com/logrhythm/generator-boreas-env/compare/v16.0.2...v16.0.3) (2021-02-15)


### Bug Fixes

* **cluster:** fix provisioning cluster for kops 1.19 ([2275bfa](https://github.com/logrhythm/generator-boreas-env/commit/2275bfaeec14637f6fe0669dfd6708282aeab588))

## [16.0.2](https://github.com/logrhythm/generator-boreas-env/compare/v16.0.1...v16.0.2) (2021-02-15)


### Bug Fixes

* **cluster-kops-update:** not updating cluster-config.json after a --reconfigure-kops run ([9bbf346](https://github.com/logrhythm/generator-boreas-env/commit/9bbf3466a28897db17c4efbdf9ba60715d2c85de))

## [16.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v16.0.0...v16.0.1) (2021-02-15)


### Bug Fixes

* update default workload config ([545b0cb](https://github.com/logrhythm/generator-boreas-env/commit/545b0cb471c398aec789b87481c8b7d4897252ba))

# [16.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v15.0.0...v16.0.0) (2021-02-11)


### Bug Fixes

* Update kops infra-module reference to released version ([0f58682](https://github.com/logrhythm/generator-boreas-env/commit/0f586828e298281866276456e5ca621f9fa850c3))


* feat!: update to kops 1.19 ([c57d30d](https://github.com/logrhythm/generator-boreas-env/commit/c57d30df72d4c8325ce6e98d4bc2adc6530f3cba))


### BREAKING CHANGES

* kops has been upgraded to 1.19

Please use kops 1.19

# [15.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v14.2.1...v15.0.0) (2021-02-09)


* feat!: update the structure of workload-config.json ([26b5a9b](https://github.com/logrhythm/generator-boreas-env/commit/26b5a9bb6a6cc04c76bd8c06687692fdf5da5885))


### BREAKING CHANGES

* migration is needed to upgrade to this version

**Migration steps**
- Check out this version of the generator
- Set the target VPC and CLUSTER to migrate
```zsh
export VPC=vpc-01
export CLUSTER=k8s
```
- Run the migration script
```zsh
cat <<\EOF > migrate.js
const fs = require('fs')

async function main() {
  const { VPC, CLUSTER } = process.env
  const workloadDirs = fs.readdirSync(`${VPC}/clusters/${CLUSTER}/kubernetes`, { withFileTypes: true })
    .filter(dirent => dirent.isDirectory())
    .map(dirent => dirent.name)
  for (const workloadName of workloadDirs) {
    const workloadConfigPath = `${VPC}/clusters/${CLUSTER}/kubernetes/${workloadName}/workload-config.json`
    if (fs.existsSync(workloadConfigPath)) {
      const workloadConfig = JSON.parse(fs.readFileSync(workloadConfigPath))
      if (workloadConfig.imageTag && workloadConfig.repository) {
        workloadConfig.images = [
          {
            name: workloadConfig.repository,
            tag: workloadConfig.imageTag
          }
        ]
        delete workloadConfig.imageTag
        delete workloadConfig.repository
      }
      if (workloadName === 'logrhythm-system') {
        workloadConfig.images = [
          {
            name: '743123016525.dkr.ecr.us-west-2.amazonaws.com/logrhythm-ops/logrhythm-operator',
            tag: workloadConfig.imageTag
          }
        ]
        delete workloadConfig.imageTag
      }
      fs.writeFileSync(workloadConfigPath, JSON.stringify(workloadConfig, null, 2))
    }
  }
}

main()
EOF

node migrate.js && rm migrate.js
```
- Then run
```zsh
yo boreas-env:cluster-workload-update --vpc $VPC --cluster $CLUSTER
```

## [14.2.1](https://github.com/logrhythm/generator-boreas-env/compare/v14.2.0...v14.2.1) (2021-02-09)


### Bug Fixes

* update default workload config ([de5ded9](https://github.com/logrhythm/generator-boreas-env/commit/de5ded9a2a80f7be32ac51452f687045e2584d52))

# [14.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v14.1.1...v14.2.0) (2021-02-08)


### Features

* add siem-ui to cors origins ([2589b01](https://github.com/logrhythm/generator-boreas-env/commit/2589b015ae86c74a7dc76a37a79a18fd2762dd6b))

## [14.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v14.1.0...v14.1.1) (2021-02-08)


### Bug Fixes

* Add updated gRPC route used to convert apiKeys to tokens ([c1f10dd](https://github.com/logrhythm/generator-boreas-env/commit/c1f10dde7bf7c3d9673f7ff82dbe3bd7bf39edec))

# [14.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v14.0.1...v14.1.0) (2021-02-05)


### Features

* **keycloak:** disable theme cacheing ([9013494](https://github.com/logrhythm/generator-boreas-env/commit/901349435f179f6d310358464f66ccbf5c78abec))

## [14.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v14.0.0...v14.0.1) (2021-02-05)


### Bug Fixes

* update default workload config ([33333b7](https://github.com/logrhythm/generator-boreas-env/commit/33333b708c99a4905e5fb8fac99892cb07c41a97))

# [14.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.9.0...v14.0.0) (2021-02-05)


### Bug Fixes

* bump default version of logrhythm-operator to 0.22.0 ([83c872d](https://github.com/logrhythm/generator-boreas-env/commit/83c872d349afdd6b871f80a9650d2a1ae15ec672))


* feat!: update logrhythm-operator templates for compatibility with version 0.22.0 ([9e8e69e](https://github.com/logrhythm/generator-boreas-env/commit/9e8e69eb5127e34821dba168f641758425304320))


### BREAKING CHANGES

* need to use logrhythm-operator docker image version 0.22.0 or higher after this version of the generator

# [13.9.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.8.0...v13.9.0) (2021-02-03)


### Features

* added kiali workload ([a1c2168](https://github.com/logrhythm/generator-boreas-env/commit/a1c21686a48a622f93e42d81826fd5e3d5634db4))
* removed pass_identity_headers in Kiali ([c101613](https://github.com/logrhythm/generator-boreas-env/commit/c10161397833163868efef28ff8366d140c90e96))

# [13.8.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.7.1...v13.8.0) (2021-02-03)


### Features

* remove agent-management-svc ([8eabe04](https://github.com/logrhythm/generator-boreas-env/commit/8eabe0412df04911576858fccd1a82d4279653ff))

## [13.7.1](https://github.com/logrhythm/generator-boreas-env/compare/v13.7.0...v13.7.1) (2021-02-02)


### Bug Fixes

* update default workload config ([29bffaa](https://github.com/logrhythm/generator-boreas-env/commit/29bffaae4d61a57719316082b32f035c3114a638))

# [13.7.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.6.0...v13.7.0) (2021-02-01)


### Features

* add capabilities for signal-processing-pipeline-svc and remove the token from the service CR ([ab73117](https://github.com/logrhythm/generator-boreas-env/commit/ab73117f9885514ff0432629781e6ebb29cefe35))

# [13.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.5.0...v13.6.0) (2021-01-28)


### Features

* making region dynamic in common tf vars ([f53b7e6](https://github.com/logrhythm/generator-boreas-env/commit/f53b7e6b980679a76213f02acd4272d579d5506a))
* updating the region for common variables ([eef1f4a](https://github.com/logrhythm/generator-boreas-env/commit/eef1f4ae3dd7d0b9709a430f10f08db3fa87c9b6))
* updating the region for common variables and index for the value ([a99491d](https://github.com/logrhythm/generator-boreas-env/commit/a99491d208e2dc554e625d89f82b2ad7c961bf1d))

# [13.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.4.1...v13.5.0) (2021-01-28)


### Bug Fixes

* removed serviceAccount and changed vault path ([1f86e99](https://github.com/logrhythm/generator-boreas-env/commit/1f86e997968723a14e93f0fb982673a86aa6ccca))


### Features

* add scheduling-svc ([cc06d8d](https://github.com/logrhythm/generator-boreas-env/commit/cc06d8df8066bfa1104ee8a0e7106d6c0bd4537d))
* enable different service prefix ([e9c2ae5](https://github.com/logrhythm/generator-boreas-env/commit/e9c2ae560ad25f2463b2edabe6d61b67b653d24e))

## [13.4.1](https://github.com/logrhythm/generator-boreas-env/compare/v13.4.0...v13.4.1) (2021-01-28)


### Bug Fixes

* update default workload config ([8cccf62](https://github.com/logrhythm/generator-boreas-env/commit/8cccf62d7fbaca3ab0eb39b7dfb7f827c533d970))

# [13.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.3.1...v13.4.0) (2021-01-26)


### Features

* added dev env's export to boreas realm ([8368c64](https://github.com/logrhythm/generator-boreas-env/commit/8368c644ec1e9dfce74fc363d88cf276251c6d2c))
* added Email Theme to Boreas Realm in Keycloak ([882b2cb](https://github.com/logrhythm/generator-boreas-env/commit/882b2cb1a4e5a658e60b3a50b9edf0d0a431f7c1))
* Final template update ([7ece967](https://github.com/logrhythm/generator-boreas-env/commit/7ece967f818ef4eb3dbbeab3a4a555fc928e8a17))
* updated all templetes ([e4a70f4](https://github.com/logrhythm/generator-boreas-env/commit/e4a70f4a345025de76c18f989ce91830e983078f))
* updated back to templete ([d4276e0](https://github.com/logrhythm/generator-boreas-env/commit/d4276e09777a454b7a921716e9177f4ccde0b13d))

## [13.3.1](https://github.com/logrhythm/generator-boreas-env/compare/v13.3.0...v13.3.1) (2021-01-25)


### Bug Fixes

* update notification-svc mailer address ([338cb87](https://github.com/logrhythm/generator-boreas-env/commit/338cb87b44e2431f9d8199fbbd87531385f83f7d))

# [13.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.2.0...v13.3.0) (2021-01-25)


### Features

* Support configurable trace sampling ([6b2ed6a](https://github.com/logrhythm/generator-boreas-env/commit/6b2ed6a81afb2fd63320b04ea1feb0c67860ef65))

# [13.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.1.0...v13.2.0) (2021-01-22)


### Features

* Remove old items from data-dictionary-svc CR applicationProperties ([785e4e4](https://github.com/logrhythm/generator-boreas-env/commit/785e4e4c75b53a247b1f052e1cf62f14eed2b840))

# [13.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v13.0.0...v13.1.0) (2021-01-22)


### Features

* Add exception-q config to signal-processing-pipeline-svc ([8a3456e](https://github.com/logrhythm/generator-boreas-env/commit/8a3456e551474bc35206a4efd60a7dfa80eb2b62))

# [13.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.14.4...v13.0.0) (2021-01-21)


### Features

* remove the manual API Key in some LogRhythmService CRs as it is now handled automatically by the lr-operator ([22dd8ab](https://github.com/logrhythm/generator-boreas-env/commit/22dd8abb1d9ac41901f0b38daa0b496a1b44f5bd))
* update logrhythm-operator version to the latest ([216a62c](https://github.com/logrhythm/generator-boreas-env/commit/216a62cd1ff8f1c2cd80dfe96642ce4e4ce83c1a))


* feat!: update logrhythm-operator workload to the latest version ([95182c0](https://github.com/logrhythm/generator-boreas-env/commit/95182c04b7bc417f8e96de772b1e8516498f6e8e))


### BREAKING CHANGES

* need to destroy and re-deploy logrhythm-operator and must use lr-operator version 0.20.0 or higher

## [12.14.4](https://github.com/logrhythm/generator-boreas-env/compare/v12.14.3...v12.14.4) (2021-01-20)


### Bug Fixes

* update default workload config ([4f51ab0](https://github.com/logrhythm/generator-boreas-env/commit/4f51ab026215c883dc92cef1b96bb0e3b126ef02))

## [12.14.3](https://github.com/logrhythm/generator-boreas-env/compare/v12.14.2...v12.14.3) (2021-01-20)


### Bug Fixes

* remove quotes from apikey ([2dc764a](https://github.com/logrhythm/generator-boreas-env/commit/2dc764a8a232b47c268c103632dcceffe0549caa))

## [12.14.2](https://github.com/logrhythm/generator-boreas-env/compare/v12.14.1...v12.14.2) (2021-01-20)


### Bug Fixes

* remove quotes from apikey ([2c38aa4](https://github.com/logrhythm/generator-boreas-env/commit/2c38aa47c8117f2b567c87a796a71c7c49cd3e07))

## [12.14.1](https://github.com/logrhythm/generator-boreas-env/compare/v12.14.0...v12.14.1) (2021-01-20)


### Bug Fixes

* update config versions for recently modified services ([4f29bb5](https://github.com/logrhythm/generator-boreas-env/commit/4f29bb53e13396a4bfa2e063dad0f8ccc07f22fd))

# [12.14.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.13.0...v12.14.0) (2021-01-20)


### Bug Fixes

* update kustomize ([600c63d](https://github.com/logrhythm/generator-boreas-env/commit/600c63d09b13e1e580adb7f5cd0872fbfbbd5094))


### Features

* add api key properties to several services ([9a18581](https://github.com/logrhythm/generator-boreas-env/commit/9a185812ea6b80c5a0bea2cde3e227cc23aaf458))
* filter-svc ([4078e57](https://github.com/logrhythm/generator-boreas-env/commit/4078e574270c81b2d9b59683ce3064ca9fa54863))

# [12.13.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.12.0...v12.13.0) (2021-01-19)


### Features

* add dependencies to signal-processing-pipeline ([4101051](https://github.com/logrhythm/generator-boreas-env/commit/41010511dac2e354458dab16fe1950fb53f2575a))

# [12.12.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.11.0...v12.12.0) (2021-01-14)


### Features

* add ACS notification-svc dependency ([c481043](https://github.com/logrhythm/generator-boreas-env/commit/c481043d113cebea4b17d0f928eae736e577d32f))

# [12.11.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.10.0...v12.11.0) (2021-01-13)


### Features

* deploy collector MFE ([9d9875f](https://github.com/logrhythm/generator-boreas-env/commit/9d9875f64431eed3b60b37c11a4a2ced4992ebdd))

# [12.10.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.9.2...v12.10.0) (2021-01-12)


### Features

* add an AlertRule for streaming-aggregation-app ([763a7e8](https://github.com/logrhythm/generator-boreas-env/commit/763a7e8ee1c99a686f18ca60a268d834c32a1eef))

## [12.9.2](https://github.com/logrhythm/generator-boreas-env/compare/v12.9.1...v12.9.2) (2021-01-12)


### Bug Fixes

* enabling debug log to Loki ([cfe1eaf](https://github.com/logrhythm/generator-boreas-env/commit/cfe1eafb709176f845996bb055f7beec6f68bc14))

## [12.9.1](https://github.com/logrhythm/generator-boreas-env/compare/v12.9.0...v12.9.1) (2021-01-12)


### Bug Fixes

* notification-svc version should be in quotes ([651e5a5](https://github.com/logrhythm/generator-boreas-env/commit/651e5a50a08f717110b4e7032ec14aba2df43894))

# [12.9.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.8.0...v12.9.0) (2021-01-12)


### Bug Fixes

* bump env to initiate rollout for notification-svc ([e983b47](https://github.com/logrhythm/generator-boreas-env/commit/e983b4750118e0c2f80fbfea9953b1b4b31be28a))


### Features

* add apispec to notification-svc ([9c31f59](https://github.com/logrhythm/generator-boreas-env/commit/9c31f591a35ec1bda5dc03b37eb04b525278e22a))

# [12.8.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.7.1...v12.8.0) (2021-01-12)


### Bug Fixes

* signal-ident host url ([ced3fc2](https://github.com/logrhythm/generator-boreas-env/commit/ced3fc2a946d0f6a2d5743c9688c0856ac8825f5))


### Features

* enable content-management-svc to communicate to signal-identification-svc over http ([d2b92d8](https://github.com/logrhythm/generator-boreas-env/commit/d2b92d8b35156276de81a8dc1d5895cb5c5ad3d8))

## [12.7.1](https://github.com/logrhythm/generator-boreas-env/compare/v12.7.0...v12.7.1) (2021-01-11)


### Reverts

* "feat: enable CMS to communicate with Signal-Ident" ([8c4b51f](https://github.com/logrhythm/generator-boreas-env/commit/8c4b51f5b5d643908f8b6ce2ed07da997e643f5d))

# [12.7.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.6.1...v12.7.0) (2021-01-11)


### Features

* enable CMS to communicate with Signal-Ident ([2c9129f](https://github.com/logrhythm/generator-boreas-env/commit/2c9129f4a0d580b223e38baee91e29c5c5bc197c))

## [12.6.1](https://github.com/logrhythm/generator-boreas-env/compare/v12.6.0...v12.6.1) (2021-01-11)


### Bug Fixes

* update default workload config ([16758ef](https://github.com/logrhythm/generator-boreas-env/commit/16758ef6607c50d45734fe30ebf2d0d6ff8c3f41))

# [12.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.5.1...v12.6.0) (2021-01-11)


### Features

* Correct quoting of componentDependencies version to match CRD type definition of "string" ([2773d1d](https://github.com/logrhythm/generator-boreas-env/commit/2773d1da8ce07eb0d801229ca4de6c6822cc4af3))
* Update logrhythm-operator config definition, including CRD, to incorporate new entries ([88ef3ce](https://github.com/logrhythm/generator-boreas-env/commit/88ef3cec6be1bf90a80052a06cf2c06a9539c053))

## [12.5.1](https://github.com/logrhythm/generator-boreas-env/compare/v12.5.0...v12.5.1) (2021-01-08)


### Bug Fixes

* bump keycloak and postgres workloads ([e514cc6](https://github.com/logrhythm/generator-boreas-env/commit/e514cc6d5fa2a59c645e09e8600e9e7b6d29491c))

# [12.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.4.0...v12.5.0) (2021-01-08)


### Features

* enable TimescaleDB for streaming-agg-app ([d46abdd](https://github.com/logrhythm/generator-boreas-env/commit/d46abdd077b984c3d805786fb773a64ca2c17e62))

# [12.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.3.0...v12.4.0) (2021-01-08)


### Features

* upgrade postgres-operator workload to v4.1.0 ([9ea9f39](https://github.com/logrhythm/generator-boreas-env/commit/9ea9f398f48311984460fc4755666b21a0f69137))

# [12.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.2.4...v12.3.0) (2021-01-08)


### Features

* enable notification-svc to communicate with cms ([aab6720](https://github.com/logrhythm/generator-boreas-env/commit/aab67206a637a6063f3c464a8debc630e00edcd8))

## [12.2.4](https://github.com/logrhythm/generator-boreas-env/compare/v12.2.3...v12.2.4) (2021-01-07)


### Bug Fixes

* Correct naming of mailhog TCP port to make istio happy ([3935958](https://github.com/logrhythm/generator-boreas-env/commit/3935958c2e17e66e68861fb130916819d5348489))

## [12.2.3](https://github.com/logrhythm/generator-boreas-env/compare/v12.2.2...v12.2.3) (2021-01-05)


### Bug Fixes

* update default workload config ([8c2a694](https://github.com/logrhythm/generator-boreas-env/commit/8c2a6947d123ad0f752639b12a08203e13df4ced))

## [12.2.2](https://github.com/logrhythm/generator-boreas-env/compare/v12.2.1...v12.2.2) (2021-01-05)


### Bug Fixes

* add dummy url to allow alert-manager to run ([bb11fe2](https://github.com/logrhythm/generator-boreas-env/commit/bb11fe2ea1c702999eb61983672a3caec02f4200))

## [12.2.1](https://github.com/logrhythm/generator-boreas-env/compare/v12.2.0...v12.2.1) (2021-01-04)


### Bug Fixes

* removed hardcoded slack channel ([4f5fb3b](https://github.com/logrhythm/generator-boreas-env/commit/4f5fb3b0a8e610e923b1b9bac62fdd0e21aa4f38))
* reorder keys to pass ci ([1a53db6](https://github.com/logrhythm/generator-boreas-env/commit/1a53db6a869c65f09c6a0d0d53e9657fd259f1ea))

# [12.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.1.0...v12.2.0) (2021-01-04)


### Features

* enable slack notifications for alert-manager ([5fa96d5](https://github.com/logrhythm/generator-boreas-env/commit/5fa96d511fd76c65263d129022135dc3a55364ec))

# [12.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v12.0.1...v12.1.0) (2021-01-04)


### Features

* upgrade lr-operator to 0.18.0 ([344e2da](https://github.com/logrhythm/generator-boreas-env/commit/344e2da3da10d148525ba964d56f0866607be283))

## [12.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v12.0.0...v12.0.1) (2020-12-31)


### Bug Fixes

* suggested cluster name none for non-shared and shared-services for shared non personal envs ([b5e5418](https://github.com/logrhythm/generator-boreas-env/commit/b5e54180e409efb461503da07bed652e370cf8d6))

# [12.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v11.1.1...v12.0.0) (2020-12-31)


### Features

* Upgrade logrhythm-operator and migrate to service componentDependencies ([9ed14a8](https://github.com/logrhythm/generator-boreas-env/commit/9ed14a80e0b65d862cae004235269e1a7aec9558))


### BREAKING CHANGES

* update to logrhythm-operator 0.17.0 required

## [11.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v11.1.0...v11.1.1) (2020-12-30)


### Bug Fixes

* **cluster:** fix error when creating cluster without Atlantis workload ([ce5ab31](https://github.com/logrhythm/generator-boreas-env/commit/ce5ab31b6a62252642bf164006586ae6b2eb77ae))

# [11.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v11.0.0...v11.1.0) (2020-12-29)


### Features

* add okta integration configs to gitops keycloaks ([2f50727](https://github.com/logrhythm/generator-boreas-env/commit/2f50727e246f9164dfa845d40dea19744b0f1c0a))

# [11.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.25.1...v11.0.0) (2020-12-29)


* refactor!: big breaking change commit message ([4c6a294](https://github.com/logrhythm/generator-boreas-env/commit/4c6a29414e701705c582d1ba02cd91ce9ea94ce4)), closes [/github.com/logrhythm/boreas-env-development/blob/master/.github/workflows/generator-cd-deploy.yaml#L105](https://github.com//github.com/logrhythm/boreas-env-development/blob/master/.github/workflows/generator-cd-deploy.yaml/issues/L105)


### Bug Fixes

* fix failed tests and update error message ([54addb3](https://github.com/logrhythm/generator-boreas-env/commit/54addb34712898377516d69e3463ed9a40cb1da4))
* **cluster:** correct kops state bucket address ([13937a3](https://github.com/logrhythm/generator-boreas-env/commit/13937a3ce57bebad383391734086536c2ee135ff))
* **cluster-destroy:** incorrect state store passed to kops ([df57bc8](https://github.com/logrhythm/generator-boreas-env/commit/df57bc804f9ccc8d1aef500fefcbb210365d242e))
* minor fixes to prompts ([24a2227](https://github.com/logrhythm/generator-boreas-env/commit/24a222781e0ef6d86c2a14e066e30436d11d1d5f))
* update subnet version ([1297b28](https://github.com/logrhythm/generator-boreas-env/commit/1297b28f3bd169210402c8498113288a6ad57299))


### Features

* check for terraform code update when run cluster-kops-update and cluster-workload-update ([d9c5537](https://github.com/logrhythm/generator-boreas-env/commit/d9c553714fb232c67c67f0d7a1150a8b4c3d0b3d))
* **cluster:** support creating multiple VPCs and multiple K8s clusters ([cfa5c84](https://github.com/logrhythm/generator-boreas-env/commit/cfa5c847b42b9fabd1dce7a1800452821209706f))
* **cluster-destroy:** support multiple VPCs and K8s Clusters ([f5a5522](https://github.com/logrhythm/generator-boreas-env/commit/f5a55225fd75d92bb3845dabb816e58417fff51f))
* **cluster-kops-update:** support multiple VPCs and K8s Clusters and add enhancements ([a432876](https://github.com/logrhythm/generator-boreas-env/commit/a4328765e2f71026cd8d2614d8f968169cfbf276))


### BREAKING CHANGES

* support multiple VPCs and K8s clusters

#### Changes to the generator:
- `yo boreas-env` now only generates some global config files for the entire environment. No VPCs, subnets, kops terraform are generated/executed in this generator. The generation and execution of terraform code is now handled by the sub-generator "terraform" but that generator will be called internally by `yo boreas-env:cluster`.
- `yo boreas-env:cluster` now handles the full cycle of VPC and cluster creation including:
  - Create all terraform code (for VPCs, Subnets, and Kops resources), and execute terraform plan <= **We now also have the ability to customize terraform code based on selected workloads or cluster configurations. In this PR, I made a change that the workload IAM Role is created based on selected workloads instead of always creating a fixed set of workload IAM roles.**
  - Generate Kops template based on the chosen version of kops configuration template, and create Kops cluster (calling `kops` command directly in the generator instead of call `./kubernetes-base/kops/create-cluster.sh`)
  - Bootstrap the cluster (pretty much the same as before)
-  `yo boreas-env:cluster-update` has been renamed to `yo boreas-env:cluster-workload-update`. Also, suggested by the name, it now **only updates k8s workloads' descriptors. This generator won't touch `kops` configuration.**
- `yo boreas-env:cluster-kops-update` now manages the full cycle of updating kops which added 2 steps to **allow user to choose a version of kops configuration template**, and update `kops/values.yaml` and `kops/cluster.yaml` accordingly before executing kops update/rolling-update.
- `yo boreas-env:cluster-destroy` now **also destroys terraform layer of the cluster** (infra/kops)
- `cluster-destroy`, `cluster-workload-update`, `cluster-kops-update` now all require `--vpc` and `--cluster` to be provided. (An enhancement can be added to prompt for vpc and cluster in the future)

#### Changes to the structure of GitOps repo:
- Environment configuration (`environment-config.json`) now stores information about all VPCs and clusters in each VPC and other shared configurations
  ```json
  {
    "personal_sandbox": true,
    "aws_account_id": "417876067775",
    "environment": "sandbox",
    "namespace": "ln-v2",
    "tf_state_s3_bucket": "ln-v2-sandbox-terraform-state",
    "gitops_repo_https": "https://github.com/tobernguyen/boreas-env-sandbox.git",
    "vpcs": {
      "vpc-ss": {
        "is_shared_services": true,
        "cidr": "10.44.0.0/16",
        "clusters": {
          "long-ss": {}
        },
        "region": "us-west-2",
        "generator_version": "10.22.1"
      },
      "vpc-01": {
        "is_shared_services": false,
        "cidr": "10.38.0.0/16",
        "region": "us-west-2",
        "generator_version": "10.22.1",
        "clusters": {
          "longn": {},
          "longn-2": {}
        }
      }
    }
  }
  ```
- Cluster configuration (`cluster-config.json`) now stores the version (commit SHA) of kops configuration template
  ```
  {
    "kops_template_version": "85153c001fe537e57fda07266605a6701fd15e05",
    "workloads": [
      "access-control-svc",
      "argocd",
      ...
    ]
  }
  ```
- `kubernetes-base` git-submodule has been removed as we are now versioning k8s workloads using "kustomize remote target" and versioning kops configuration template discretely using the generator.

#### Changes to Local Dev (Cloud Engineer):
- New quick command to destroy your sandbox
  ```zsh
  yo boreas-env:cluster-destroy --vpc VPC_DIR_NAME --cluster CLUSTER_SHORT_NAME --skip-confirm
  ```
- New quick command to rebuild your sandbox
  ```zsh
  yo boreas-env:cluster --vpc VPC_DIR_NAME --cluster CLUSTER_SHORT_NAME --skip-confirm
  ```
- Some other changes to the dev workflow/experience like developing/updating/testing k8s workload or kops configuration template (due to the removal of `kubernetes-base` and command changes)

**Migration steps for existing environments**

- Check out this version of the generator
- Go to the target GitOps repo, run
  ```zsh
  cat <<\EOF > migrate.js
  const fs = require('fs')

  function pick(object, keys) {
    return keys.reduce((obj, key) => {
      if (object && object.hasOwnProperty(key)) {
          obj[key] = object[key];
      }
      return obj;
    }, {});
  }

  function main() {
    const envConfig = require('./environment-config.json')
    const clusterPath = `./${envConfig.vpc_dir_name}/clusters/${envConfig.cluster_short_name}/cluster-config.json`
    const clusterConfig = require(`${clusterPath}`)

    const newEnvConfig = Object.assign(
      pick(envConfig,
      [
        'personal_sandbox',
        'aws_account_id',
        'environment',
        'namespace',
        'tf_state_s3_bucket',
      ]),
      {
        gitops_repo_https: clusterConfig.gitops_repo_https,
        vpcs: {
          [envConfig.vpc_dir_name]: {
            is_shared_services: false,
            cidr: envConfig.cidr,
            region: 'us-west-2',
            generator_version: '11.0.0',
            clusters: {
              [envConfig.cluster_short_name]: {}
            }
          }
        }
      }
    )

    const { gitops_repo_https, ...newClusterConfig } = clusterConfig
    Object.assign(
      newClusterConfig,
      {
        kops_template_version: '85153c001fe537e57fda07266605a6701fd15e05' // boreas-kubernetes tag v4.0.1
      }
    )

    fs.writeFileSync('./environment-config.json', JSON.stringify(newEnvConfig, null, 2))
    fs.writeFileSync(clusterPath, JSON.stringify(newClusterConfig, null, 2))
    fs.unlinkSync('./.gitmodules')
    fs.rmdirSync('./kubernetes-base', { recursive: true })
    fs.unlinkSync('./migrate.js')
  }

  main()
  EOF

  node migrate.js
  ```
- Run
  ```zsh
  export VPC=VPC_DIR_NAME
  export CLUSTER=CLUSTER_SHORT_NAME

  yo boreas-env # Update shared files
  yo boreas-env:terraform --vpc $VPC --cluster $CLUSTER --skip-tf-run # Update terraform code. For personal sandboxes, you can remove "--skip-tf-run" so that the generator will apply terraform changes locally.
  yo boreas-env:cluster-kops-update --vpc $VPC --cluster $CLUSTER # Update kops templates and execute kops update
  yo boreas-env:cluster-workload-update --vpc $VPC --cluster $CLUSTER # Update k8s workloads
  ```
- Make sure to push changes to GitOps repo
- Now the environment is migrated, we should be able to use the new version of the generator for this environment from now on.

**Migration steps for CD Pipeline in boreas-env-development**

## [10.25.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.25.0...v10.25.1) (2020-12-29)


### Bug Fixes

* update default docs imageTag so it reflects the current FRONTEND_COMPONENT_IMAGE_TAG_PATTERN in check-workload-update.js ([6599d25](https://github.com/logrhythm/generator-boreas-env/commit/6599d2531c72530b69a7e80b4fabbdb8a4b12ec0))

# [10.25.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.24.0...v10.25.0) (2020-12-29)


### Features

* adding a group for ses_smtp users ([5370ef6](https://github.com/logrhythm/generator-boreas-env/commit/5370ef68ddbc21b3c227c7d37c8b7902555e1b68))

# [10.24.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.23.1...v10.24.0) (2020-12-28)


### Bug Fixes

* update imageTag to latest working version ([21dc27f](https://github.com/logrhythm/generator-boreas-env/commit/21dc27fa4d2cd88035d13050026d0589eb39f1af))


### Features

* adding docs workload ([3d927e8](https://github.com/logrhythm/generator-boreas-env/commit/3d927e8af802afe10b3d6e59f916d937737b2942))

## [10.23.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.23.0...v10.23.1) (2020-12-23)


### Bug Fixes

* increase max node count to enable upgrades ([4a82366](https://github.com/logrhythm/generator-boreas-env/commit/4a8236625df01d8908fe02cc727bba7c7986ddab))

# [10.23.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.22.2...v10.23.0) (2020-12-23)


### Features

* add topology-svc ([283ae23](https://github.com/logrhythm/generator-boreas-env/commit/283ae23a2f932392f06a775c42bfb47df9e13a05))

## [10.22.2](https://github.com/logrhythm/generator-boreas-env/compare/v10.22.1...v10.22.2) (2020-12-22)


### Bug Fixes

* increase data node size ([f26da6a](https://github.com/logrhythm/generator-boreas-env/commit/f26da6a21df1e344195d429838bcc31408bbac2d))

## [10.22.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.22.0...v10.22.1) (2020-12-22)


### Bug Fixes

* update default workload config ([01b932a](https://github.com/logrhythm/generator-boreas-env/commit/01b932ab60c76c5124c36648f2ae0d446b4df1a1))

# [10.22.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.21.3...v10.22.0) (2020-12-21)


### Features

* increase number of partitions for audit and signal-ingest from 3 to 16 ([9051cfb](https://github.com/logrhythm/generator-boreas-env/commit/9051cfb28c15f9f4eab44767001aa7c8b582bffe))

## [10.21.3](https://github.com/logrhythm/generator-boreas-env/compare/v10.21.2...v10.21.3) (2020-12-21)


### Bug Fixes

* increase liveness probe for sis ([be37d03](https://github.com/logrhythm/generator-boreas-env/commit/be37d0345c50c957d93430d3bae59a5ba052f6ce))

## [10.21.2](https://github.com/logrhythm/generator-boreas-env/compare/v10.21.1...v10.21.2) (2020-12-21)


### Bug Fixes

* remove extra space in realms-volume.yaml ([7fd64cb](https://github.com/logrhythm/generator-boreas-env/commit/7fd64cb9d481f1fd002f296d9d3e1ad15607b43d))

## [10.21.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.21.0...v10.21.1) (2020-12-18)


### Bug Fixes

* update default workload config ([576be13](https://github.com/logrhythm/generator-boreas-env/commit/576be13486598e33bb1a5dbee5e71a993d5941b1))

# [10.21.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.20.4...v10.21.0) (2020-12-16)


### Bug Fixes

* logrhythm_okta realm will now import ([3fe021c](https://github.com/logrhythm/generator-boreas-env/commit/3fe021cc9166c5c742cc0bd74af1b41812959219))
* pomerium secret templating in realms.yaml.operations and STARTUP_ARGUMENTS ([9bcb045](https://github.com/logrhythm/generator-boreas-env/commit/9bcb04569360fd4d19cb292e77a6e031d6bdca61))
* remove client secret templating ([1b59dfa](https://github.com/logrhythm/generator-boreas-env/commit/1b59dfa1cbf9f5676f2a342c55b6b5d8835f4717))


### Features

* add logrhythm_okta realm and okta idp configs ([5443be5](https://github.com/logrhythm/generator-boreas-env/commit/5443be50e579185d46df94ee4e2e7d3cace2127d))

## [10.20.4](https://github.com/logrhythm/generator-boreas-env/compare/v10.20.3...v10.20.4) (2020-12-15)


### Bug Fixes

* update default workload config ([6c636bd](https://github.com/logrhythm/generator-boreas-env/commit/6c636bd1a58d57a477e75730fa0ba8f2732d7975))

## [10.20.3](https://github.com/logrhythm/generator-boreas-env/compare/v10.20.2...v10.20.3) (2020-12-11)


### Bug Fixes

* update default workload config ([623d82a](https://github.com/logrhythm/generator-boreas-env/commit/623d82affe8d300b20d6cd8a897d506a9289d4d8))

## [10.20.2](https://github.com/logrhythm/generator-boreas-env/compare/v10.20.1...v10.20.2) (2020-12-10)


### Bug Fixes

* update default workload config ([a9dd25e](https://github.com/logrhythm/generator-boreas-env/commit/a9dd25eb58b10088dfc889945b6a0503ef180a4b))

## [10.20.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.20.0...v10.20.1) (2020-12-08)


### Bug Fixes

* update default workload config ([f7ed2b2](https://github.com/logrhythm/generator-boreas-env/commit/f7ed2b222ba448464b9ba9775c1dc7ab50999f0b))

# [10.20.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.19.0...v10.20.0) (2020-12-08)


### Bug Fixes

* **vault:** fix spacing issue ([3224184](https://github.com/logrhythm/generator-boreas-env/commit/3224184732f33cb0756b9ae3ab1e61aa8063ed8d))
* **vault:** minor refactors and fix spacing issues ([3bea713](https://github.com/logrhythm/generator-boreas-env/commit/3bea71347a885b906449a7954750ffb283584ac2))


### Features

* **vault:** DRY infinispan policies ([82637c9](https://github.com/logrhythm/generator-boreas-env/commit/82637c9a8d54a139b3cefca66b575168c8d62f98))
* **vault:** Support dynamic generation of Vault policies per definitions in workloads.js ([b12b8d8](https://github.com/logrhythm/generator-boreas-env/commit/b12b8d8801b68c8c38a74e2a7c7249c345f1b730))

# [10.19.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.18.0...v10.19.0) (2020-12-07)


### Features

* Update logrhythm-operator version ([877cf96](https://github.com/logrhythm/generator-boreas-env/commit/877cf964247de3167ffce2446f47d62d7409cbd8))

# [10.18.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.8...v10.18.0) (2020-12-07)


### Features

* Add boreas token to search-index and data-dictionary, along with data-dictionary client config in search-indexing ([9c2a572](https://github.com/logrhythm/generator-boreas-env/commit/9c2a572e7a4608c672ce1adb3d253f8ee113e7f8))
* Upgrade from Elastic 7.8.0 -> 7.10.0 ([aabd56f](https://github.com/logrhythm/generator-boreas-env/commit/aabd56f079959815d96d40f8824ad2d4521cc84d))

## [10.17.8](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.7...v10.17.8) (2020-12-07)


### Bug Fixes

* case where user selects atlantis workload to install and correctly prompt for github credentials. ([38a3c2d](https://github.com/logrhythm/generator-boreas-env/commit/38a3c2d79b3e72f3f2d5b71e04d0a5f814580a7e))
* linting ([8836f2d](https://github.com/logrhythm/generator-boreas-env/commit/8836f2dc04ed5558b2f9204730e546757c547dd9))

## [10.17.7](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.6...v10.17.7) (2020-12-02)


### Bug Fixes

* update default workload config ([74c93d8](https://github.com/logrhythm/generator-boreas-env/commit/74c93d8b242d4c6031aa720c48ae6869cbee9b08))

## [10.17.6](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.5...v10.17.6) (2020-11-27)


### Bug Fixes

* update default workload config ([3952e5a](https://github.com/logrhythm/generator-boreas-env/commit/3952e5ad07cdc4e9908be97d44ebbb5c103c10c6))

## [10.17.5](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.4...v10.17.5) (2020-11-25)


### Bug Fixes

* update default workload config ([000e78a](https://github.com/logrhythm/generator-boreas-env/commit/000e78a8d781d81b928f8baba9517fb0d247c81b))

## [10.17.4](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.3...v10.17.4) (2020-11-23)


### Bug Fixes

* update default workload config ([4df2f32](https://github.com/logrhythm/generator-boreas-env/commit/4df2f32f9efef70d85219d4fd8027511a132a34c))

## [10.17.3](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.2...v10.17.3) (2020-11-20)


### Bug Fixes

* update default workload config ([9e2009f](https://github.com/logrhythm/generator-boreas-env/commit/9e2009f3dd41c612690314982e30a032903e83c1))

## [10.17.2](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.1...v10.17.2) (2020-11-19)


### Bug Fixes

* DE11633: fix issue where workload is deployed in a branch, but isn't in master yet and when back on master the cluster-update errors out. ([ba317fb](https://github.com/logrhythm/generator-boreas-env/commit/ba317fb10a2bdb5cf023208e7f70d6e9971645c5))
* don't need second null check ([c566a69](https://github.com/logrhythm/generator-boreas-env/commit/c566a696b0dcce33b34dba3f1a0f279d8f83e8f8))
* ignore workload during cluster-update if it's been added in branch, but not in master ([1b68fbe](https://github.com/logrhythm/generator-boreas-env/commit/1b68fbe9c9974bdae6c4ac85a72780c14620f6fc))
* instead of automatically continuing (and therefore removing the workload in question) just throw a meaningful error ([12d9c78](https://github.com/logrhythm/generator-boreas-env/commit/12d9c7850d1306fb835e0e43da8010d6dd96a752))
* remove debug line ([ab41e67](https://github.com/logrhythm/generator-boreas-env/commit/ab41e67f3f81b7f68f90966651ed9563b53a8227))
* uncomment dds ([e523a1b](https://github.com/logrhythm/generator-boreas-env/commit/e523a1b2459e12957fc279ce285d515a6a1c4b2f))

## [10.17.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.17.0...v10.17.1) (2020-11-18)


### Bug Fixes

* update default workload config ([00db155](https://github.com/logrhythm/generator-boreas-env/commit/00db155ca783e2934b334dc2d36850815170f755))

# [10.17.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.16.1...v10.17.0) (2020-11-18)


### Features

* add a script to update default workloads’ configs from boreas-env-development ([308f031](https://github.com/logrhythm/generator-boreas-env/commit/308f03103f3a3e3a29866b9d973b6c3eb79475cc))

## [10.16.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.16.0...v10.16.1) (2020-11-17)


### Bug Fixes

* ignoreDiffereneces for lr-infinispan-prometheus-metrics-secret ([63743aa](https://github.com/logrhythm/generator-boreas-env/commit/63743aad55b21162717193cd4ec80b426140863a))

# [10.16.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.15.2...v10.16.0) (2020-11-16)


### Features

* **eck:** Add volumeClaimTemplates to all nodeSets ([c8264fb](https://github.com/logrhythm/generator-boreas-env/commit/c8264fb6f51a4f085b8448986ed53caa03f7a3dc))
* **eck:** Enable x-pack monitoring to allow viewing cluster status in Kibana ([2bacbef](https://github.com/logrhythm/generator-boreas-env/commit/2bacbefde227b2255c650520dc48a1d97e30a486))
* Allow configuration of ES data node count and volume size ([811b18f](https://github.com/logrhythm/generator-boreas-env/commit/811b18f182b2f99214d35170d83fde24a5694e7e))

## [10.15.2](https://github.com/logrhythm/generator-boreas-env/compare/v10.15.1...v10.15.2) (2020-11-16)


### Bug Fixes

* added CMS property in DDS ([e0a45ed](https://github.com/logrhythm/generator-boreas-env/commit/e0a45edd5c5df8ac538121c2a57b30a2b502b3af))
* removed whitespace ([c926da4](https://github.com/logrhythm/generator-boreas-env/commit/c926da40f37dd5878e1a77eacb9ffbbea6dd630d))

## [10.15.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.15.0...v10.15.1) (2020-11-16)


### Bug Fixes

* added missing property for data-dictionary-svc ([111ba4d](https://github.com/logrhythm/generator-boreas-env/commit/111ba4da59370fddc27036384e451892dfc440f0))
* updatng property ([c75f082](https://github.com/logrhythm/generator-boreas-env/commit/c75f082ae933840e14c22d44b943ac48fb9f7dac))

# [10.15.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.14.1...v10.15.0) (2020-11-13)


### Features

* add ability to perform a kops rolling update to the generator ([c1a8047](https://github.com/logrhythm/generator-boreas-env/commit/c1a804754c41ef0729d61c0f7f329df44263d351))
* adding documentation for cluster-kops-update ([a7ff14b](https://github.com/logrhythm/generator-boreas-env/commit/a7ff14be80d698d431bf133ff081abc3b8b7acc1))

## [10.14.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.14.0...v10.14.1) (2020-11-13)


### Bug Fixes

* Update ignored list for upgraded ECK ([d420380](https://github.com/logrhythm/generator-boreas-env/commit/d420380a9b60e792c10239ebceb442443803f2e1))
* **eck:** Ensure istio annotations are properly applied ([dde4619](https://github.com/logrhythm/generator-boreas-env/commit/dde4619df850e1e761acd266a22d180d0d35b7a2))

# [10.14.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.13.0...v10.14.0) (2020-11-06)


### Features

* enable service to use vault secret store ([45b6d24](https://github.com/logrhythm/generator-boreas-env/commit/45b6d24aecc4f936482a06b9a6e33a643a27ff24))

# [10.13.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.12.0...v10.13.0) (2020-11-06)


### Features

* add signal-relay-svc ([a058c68](https://github.com/logrhythm/generator-boreas-env/commit/a058c68d596eb9a906afc39660d930d355b637f8))

# [10.12.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.11.3...v10.12.0) (2020-11-05)


### Features

* add data-dictionary-svc workload ([5bdb1d4](https://github.com/logrhythm/generator-boreas-env/commit/5bdb1d4c6b1cd32d48551849a88d40b8a44bd64d))

## [10.11.3](https://github.com/logrhythm/generator-boreas-env/compare/v10.11.2...v10.11.3) (2020-11-04)


### Bug Fixes

* move versions into constants.js ([5572333](https://github.com/logrhythm/generator-boreas-env/commit/55723334a9336e0dd2e6a290d5f5473c6cc35e80))

## [10.11.2](https://github.com/logrhythm/generator-boreas-env/compare/v10.11.1...v10.11.2) (2020-11-03)


### Bug Fixes

* **notification-svc:** correct application properties ([9c21b10](https://github.com/logrhythm/generator-boreas-env/commit/9c21b10873516b6805b3c63eabe71a37b2d3b4de))

## [10.11.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.11.0...v10.11.1) (2020-11-03)


### Bug Fixes

* **notification-svc:** add missing application props ([71a091a](https://github.com/logrhythm/generator-boreas-env/commit/71a091ac125a2aa7f48fc60d8206852e7f1baa86))

# [10.11.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.10.0...v10.11.0) (2020-11-02)


### Features

* add kops rolling update part 1 ([448c269](https://github.com/logrhythm/generator-boreas-env/commit/448c269e2f7afbf07735b549fddf02a9f8364030))

# [10.10.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.9.2...v10.10.0) (2020-11-02)


### Features

* added troubleshooting steps ([202d26b](https://github.com/logrhythm/generator-boreas-env/commit/202d26b406ddd3df5692144db25fef511f69051a))
* added troubleshooting steps ([9caf0f7](https://github.com/logrhythm/generator-boreas-env/commit/9caf0f7732e7beed469f45b99f712058a613134b))

## [10.9.2](https://github.com/logrhythm/generator-boreas-env/compare/v10.9.1...v10.9.2) (2020-10-30)


### Bug Fixes

* flink image tag and minio sizing ([256b785](https://github.com/logrhythm/generator-boreas-env/commit/256b785446af13bf150cbcb62e4da909ea44191d))

## [10.9.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.9.0...v10.9.1) (2020-10-30)


### Bug Fixes

* support flink rolling updates ([86feacf](https://github.com/logrhythm/generator-boreas-env/commit/86feacf4081c51a4d5363c6a72c77d720bd28b65))

# [10.9.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.8.0...v10.9.0) (2020-10-28)


### Features

* add notification-svc workload ([d47f3f4](https://github.com/logrhythm/generator-boreas-env/commit/d47f3f4213889d22c5a5a69f1616478582943e52))

# [10.8.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.7.1...v10.8.0) (2020-10-28)


### Features

* **kops:** Update K8s to 1.18.10, including base AMI and remove discrete SSH keys ([84f26de](https://github.com/logrhythm/generator-boreas-env/commit/84f26de10ded7af425b1fe3ca445ed619ac2b47b))

## [10.7.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.7.0...v10.7.1) (2020-10-28)


### Bug Fixes

* **cluster-connect:** fix the flakiness connection ([b032aa5](https://github.com/logrhythm/generator-boreas-env/commit/b032aa559107a8e292a8651aedb70ab8cd137dba))

# [10.7.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.6.0...v10.7.0) (2020-10-26)


### Features

* **cluster-connect:** create temporary SSH key to SSH to Master Node via SSM ([abb3628](https://github.com/logrhythm/generator-boreas-env/commit/abb3628f006309b247b722bd6444662bcd078b51))

# [10.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.5.0...v10.6.0) (2020-10-22)


### Features

* updated ssh key ([a7f459c](https://github.com/logrhythm/generator-boreas-env/commit/a7f459cf8cf59aa8df99462ec1280373c93b6331))

# [10.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.4.0...v10.5.0) (2020-10-22)


### Features

* added agent-management-svc ([eb622de](https://github.com/logrhythm/generator-boreas-env/commit/eb622ded86e57f29cef89afc624400042431bec5))

# [10.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.3.0...v10.4.0) (2020-10-21)


### Features

* Add content-mgmt client properties in signal-normalization-svc ([08470ff](https://github.com/logrhythm/generator-boreas-env/commit/08470ff6724c7994268971d49178f2cbd9e08f3f))

# [10.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.2.0...v10.3.0) (2020-10-21)


### Features

* Add token property in signal-processing-pipeline ([2f6bfc0](https://github.com/logrhythm/generator-boreas-env/commit/2f6bfc07197a1dfa22c7e9e46371a66f5a7d93d2))

# [10.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.1.1...v10.2.0) (2020-10-20)


### Features

* **cluster-connect:** print unique argocd address for different clusters ([5936e3b](https://github.com/logrhythm/generator-boreas-env/commit/5936e3bdec0a2f9e210afe6f14674671c758d6cb))

## [10.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v10.1.0...v10.1.1) (2020-10-20)


### Bug Fixes

* Clean up unnecessary audit-svc config ([ccf3bbf](https://github.com/logrhythm/generator-boreas-env/commit/ccf3bbff057506478a22b82fc01913e657dbcc65))
* Remove 3 common configurations moved into Logrhythm Operator v0.14.1 ([5b7cab3](https://github.com/logrhythm/generator-boreas-env/commit/5b7cab36119b9f01dbc05cb96752ac32f192118f))
* Update logrhythm-operator version to expected version for these config changes ([b7b621f](https://github.com/logrhythm/generator-boreas-env/commit/b7b621f8f64e9dbb8adbbf22c7b8a9ead21209fb))
* Update signal-identification-svc config to connect to content-management-svc ([42e2334](https://github.com/logrhythm/generator-boreas-env/commit/42e23342b016a24dcff9bc249b01b844cb6a88b7))

# [10.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v10.0.0...v10.1.0) (2020-10-20)


### Features

* **vault:** add webhook role ([ea89424](https://github.com/logrhythm/generator-boreas-env/commit/ea89424b4a330afe3bb7d899b46c560f31fb6846))

# [10.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v9.4.2...v10.0.0) (2020-10-13)


### Features

* get terraform outputs from S3 instead of local file ([a2ed0b1](https://github.com/logrhythm/generator-boreas-env/commit/a2ed0b13a440f0970841a2c79388207fa565b642))


### BREAKING CHANGES

* `yo boreas-env:cluster-update` now requires valid AWS Credential set in the environment.

- For CI environment, running `yo boreas-env:cluster-update --ci` now requires AWS Credentials set in the environment. The credential should have permission to read files from Terraform State S3 Bucket.
- There is no change to the local dev workflow, all commands work the same except `yo boreas-env:cluster-update` now also requires AWS Credential and Profile set in the environment (like some other commands like `yo boreas-env:cluster`)

## [9.4.2](https://github.com/logrhythm/generator-boreas-env/compare/v9.4.1...v9.4.2) (2020-10-13)


### Bug Fixes

* remove ENVIRONMENT_PUBLIC_PATH ([b40680b](https://github.com/logrhythm/generator-boreas-env/commit/b40680b4202208f4afff037ae015d7ed1a8c3a30))

## [9.4.1](https://github.com/logrhythm/generator-boreas-env/compare/v9.4.0...v9.4.1) (2020-10-13)


### Bug Fixes

* add missing comma ([c0f6477](https://github.com/logrhythm/generator-boreas-env/commit/c0f6477d0d7239fe9759d1d5df0d75efa8069f4a))
* simplify runtimeConfig for siem-ui and keycloak login theme ([d658640](https://github.com/logrhythm/generator-boreas-env/commit/d658640a448e52286df8b134904d3d0e09e69b31))

# [9.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v9.3.1...v9.4.0) (2020-10-12)


### Features

* adding nav-suggestion-svc ([727f3be](https://github.com/logrhythm/generator-boreas-env/commit/727f3be12355f5974443d16c1f13f83541b8974b))

## [9.3.1](https://github.com/logrhythm/generator-boreas-env/compare/v9.3.0...v9.3.1) (2020-10-07)


### Bug Fixes

* typo in cms host setting ([b213144](https://github.com/logrhythm/generator-boreas-env/commit/b213144a0017f0d98d458f498d9904ba88d7f601))

# [9.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v9.2.0...v9.3.0) (2020-10-07)


### Features

* **signal-identification-svc:** adding integration with content-management-svc ([da1e352](https://github.com/logrhythm/generator-boreas-env/commit/da1e35260ca13a53e3901990914994d2c13fd7d3))

# [9.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v9.1.0...v9.2.0) (2020-10-06)


### Bug Fixes

* reordered workloads.js ([40a3d94](https://github.com/logrhythm/generator-boreas-env/commit/40a3d94c5a3b50e218dab4e4351f0e659022a470))


### Features

* add infinispan workload ([f506531](https://github.com/logrhythm/generator-boreas-env/commit/f506531525ef0647d1e6b031d03aa3e72a30d003))

# [9.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v9.0.2...v9.1.0) (2020-10-06)


### Features

* Deploy flink streaming-aggregation-app ([2c86b58](https://github.com/logrhythm/generator-boreas-env/commit/2c86b58df6f0336b760f58b6815104c2d0799981))

## [9.0.2](https://github.com/logrhythm/generator-boreas-env/compare/v9.0.1...v9.0.2) (2020-10-02)


### Bug Fixes

* **logrhythm-operator:** Reduce CPU request to 5 so it will fit on a t3a.2xlarge ([4f98d43](https://github.com/logrhythm/generator-boreas-env/commit/4f98d43766d9ba14d3a7374499330003f47ccc46))

## [9.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v9.0.0...v9.0.1) (2020-10-02)


### Bug Fixes

* **logrhythm-operator:** Set limits to account for mass CPU usage ([cbc0f51](https://github.com/logrhythm/generator-boreas-env/commit/cbc0f510bffe19396686748325dba24854b3822c))

# [9.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v8.6.0...v9.0.0) (2020-10-02)


### Bug Fixes

* ignore status field of tenants.minio.min.io CRD ([074fd51](https://github.com/logrhythm/generator-boreas-env/commit/074fd51248978f19696f38e8954b2d6a859b0830))
* make Keycloak sync after PG Operator ([ade75ef](https://github.com/logrhythm/generator-boreas-env/commit/ade75ef02cf176afbab4b1e43432abf2d19e849a))
* update new ArgoCD waves ([40b252b](https://github.com/logrhythm/generator-boreas-env/commit/40b252bb68d52ebd6122a28252a5551c4076639d))


### Features

* add MinIO workload ([1068b7a](https://github.com/logrhythm/generator-boreas-env/commit/1068b7a7a95ce5130b988f7b2cb8e06affe86c6f))
* remove Loki config from the generator as it is in kubernetes-base now ([8e99769](https://github.com/logrhythm/generator-boreas-env/commit/8e997697ef510a4474f65021bb20556f8f8c3f53))
* update new ArgoCD sync waves ([62eb38d](https://github.com/logrhythm/generator-boreas-env/commit/62eb38db05f07590f89b8e536e9401fba6689fa9))


### BREAKING CHANGES

* Loki now uses S3 as backend storage.

Migration steps: https://github.com/logrhythm/generator-boreas-env/pull/170

# [8.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v8.5.5...v8.6.0) (2020-09-29)


### Features

* Add Search MFE ([4dc7049](https://github.com/logrhythm/generator-boreas-env/commit/4dc7049fa7262c50fd45fdf64cf85e8151288c1f))

## [8.5.5](https://github.com/logrhythm/generator-boreas-env/compare/v8.5.4...v8.5.5) (2020-09-24)


### Bug Fixes

* misspelled Manoj's last name ([b993adc](https://github.com/logrhythm/generator-boreas-env/commit/b993adcc71600d4215e7291d7775b173f0f84851))

## [8.5.4](https://github.com/logrhythm/generator-boreas-env/compare/v8.5.3...v8.5.4) (2020-09-24)


### Bug Fixes

* **search-indexing-svc:** Correct ES config, adding auth and adjusting node counts ([8539b09](https://github.com/logrhythm/generator-boreas-env/commit/8539b0992b0626ac10d7aa1fe11e7938e18ebbb9))

## [8.5.3](https://github.com/logrhythm/generator-boreas-env/compare/v8.5.2...v8.5.3) (2020-09-23)


### Bug Fixes

* edit generator-tools.yaml to work with new onboarding playbook ([b91fcee](https://github.com/logrhythm/generator-boreas-env/commit/b91fceef688639559c859e00ab81c68adb1c3b6a))

## [8.5.2](https://github.com/logrhythm/generator-boreas-env/compare/v8.5.1...v8.5.2) (2020-09-21)


### Bug Fixes

* override mailhog host property ([16865c8](https://github.com/logrhythm/generator-boreas-env/commit/16865c8535988817f4de92b2e55bc9c685fa984d))

## [8.5.1](https://github.com/logrhythm/generator-boreas-env/compare/v8.5.0...v8.5.1) (2020-09-21)


### Bug Fixes

* disable automerge in atlantis config ([1b706a4](https://github.com/logrhythm/generator-boreas-env/commit/1b706a4473174ccf286d5156265e7dbd516e49a8))

# [8.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v8.4.0...v8.5.0) (2020-09-21)


### Bug Fixes

* add vault-operator to dependency list of quarkus-services-shared ([aa8b9d2](https://github.com/logrhythm/generator-boreas-env/commit/aa8b9d2a88e18c3c43fbccc7a4d6871a38a8a8d3))
* use FQDN for Vault URL ([28f481e](https://github.com/logrhythm/generator-boreas-env/commit/28f481e41df096b5e26d1b51584e7a748a88f703))


### Features

* add vault configurations to all LogRhythmService’s application.properties ([8e430c5](https://github.com/logrhythm/generator-boreas-env/commit/8e430c525fe9566435f3c228514c378e336813df))
* add vault-operator workload ([1e4bb4a](https://github.com/logrhythm/generator-boreas-env/commit/1e4bb4a1b450c094e535810f5f663a236c997004))

# [8.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v8.3.0...v8.4.0) (2020-09-17)


### Features

* add signal-identification-svc workload ([02e8230](https://github.com/logrhythm/generator-boreas-env/commit/02e8230026986fdae9bdbdcca6d510ebdfba56c7))
* add signal-normalization-svc workload ([2176213](https://github.com/logrhythm/generator-boreas-env/commit/217621306b2cdbe83ffc60802812bfbebcc60e46))

# [8.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v8.2.0...v8.3.0) (2020-09-17)


### Features

* **kops:** Enable versioning on kops s3 state bucket ([dbc089a](https://github.com/logrhythm/generator-boreas-env/commit/dbc089a348c08b98e77dbc2e1ca9ea416438f2f8))

# [8.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v8.1.0...v8.2.0) (2020-09-16)


### Features

* correct gRPC route prefix for some LR services ([e84e215](https://github.com/logrhythm/generator-boreas-env/commit/e84e21561ed91a866671dfeadced2b1934b89605))

# [8.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v8.0.1...v8.1.0) (2020-09-16)


### Bug Fixes

* linting ([493870c](https://github.com/logrhythm/generator-boreas-env/commit/493870c088078277cb77a9a482457a5be4aee778))
* remove allowed_groups, as couldn't get config to work ([98e9d94](https://github.com/logrhythm/generator-boreas-env/commit/98e9d94a640404993b950237fbec3cd2a4687ce2))
* remove identity headers - not needed ([26e6c84](https://github.com/logrhythm/generator-boreas-env/commit/26e6c84de4c915f203785bc5ebf4832a6e53cbcf))
* Update generators/cluster/templates/kubernetes/search-indexing-svc/search-indexing-svc.yaml ([817c109](https://github.com/logrhythm/generator-boreas-env/commit/817c109e45091ac65fa1c9fb4d8ba59257c13dd9))


### Features

* add auth secret definition to service CR ([e5f7184](https://github.com/logrhythm/generator-boreas-env/commit/e5f718438f9baa6205937f5410c3b81089e91625))
* add kibana virtual service and policy ([788dcc0](https://github.com/logrhythm/generator-boreas-env/commit/788dcc091a764f267adc45e403e818ea0ddafb67))

## [8.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v8.0.0...v8.0.1) (2020-09-09)


### Bug Fixes

* set SIEM UI certificate issuer based on environment ([896e3c6](https://github.com/logrhythm/generator-boreas-env/commit/896e3c6cb654c44a1522f4ccc0fcd6e407fe5ba9))

# [8.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v7.0.2...v8.0.0) (2020-09-09)


### Bug Fixes

* ignore changes in annotations in IstioOperator CRD ([7ea6e5b](https://github.com/logrhythm/generator-boreas-env/commit/7ea6e5b93545f1069f0492b359351ac32fcc4ec1))


### Features

* upgrade Istio to 1.7 and add Jaeger Operator ([4ed74df](https://github.com/logrhythm/generator-boreas-env/commit/4ed74dfd8b1a3d98021899eb392889d28cec35a4))


### BREAKING CHANGES

* upgrade Istio to 1.7, need migration

### Migration steps: Upgrade Istio from 1.4.6 to 1.7.0

0. Have your cluster up and running healthy with Istio 1.4.6

1. Disable ArgoCD auto sync policy for all applications
```zsh
APP_DIR=$(jq -r '"\(.vpc_dir_name)/clusters/\(.cluster_short_name)"' environment-config.json)/kubernetes/_argocd-apps/applications
find $APP_DIR -iname '*.yaml' -maxdepth 1 | xargs -n1 yq -y -i 'del(.spec.syncPolicy)'
```

3. Commit/Push. Go to ArgoCD Dashboard. Click refresh/sync on `apps` panel.

4. Take everything in the cluster out of service mesh
```zsh
./take-everything-out-of-mesh.sh
```

5. Wait for a few mins, go to your cluster to confirm that all deploy/sts are out of mesh (no envoy sidecar container). Note: Elasticsearch takes a while to rolling restart all pods.

NOTE: Unleash is the only service that is not healthy after this step, we don't know why. But to make it healthy again, we might need to drop Unleash's pg database.

And also we can't access to services that have destination rule set to ISTIO_MUTUAL

6. Go to ArgoCD Dashboard, delete `istio-system` there. Go to your cluster, confirm that `istio-system` namespace is terminated. If not, delete `istio-system` namespace

7. Run `yo boreas-env:cluster-update` to have the latest boreas-kubernetes ref (branch that has new kops template and Istio 1.7). DON'T PUSH CHANGES YET.

8. Do rolling update for kops.

9. Push changes to GitOps. Go to ArgoCD, manually sync `istio-system` application

10. Confirm istio 1.7 is up and healthy.

11. Run script
```zsh
./mesh-again.sh
```

12. Go to ArgoCD and sync everything again

13. Confirm deploy/sts is running with istio 1.7 sidecar container injected

14. We might need to delete Unleash pg cluster for Unleash to work again

15. We might need re-roll Pomerium too

15. Confirm jaeger is up and running

## [7.0.2](https://github.com/logrhythm/generator-boreas-env/compare/v7.0.1...v7.0.2) (2020-09-09)


### Bug Fixes

* **search-indexing-svc:** Add config for correct Kafka topic consumption ([cf53134](https://github.com/logrhythm/generator-boreas-env/commit/cf5313492227d16ad627b4d41ddbeacf6b20940f))

## [7.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v7.0.0...v7.0.1) (2020-09-08)


### Bug Fixes

* define retention settings for loki ([f4b0998](https://github.com/logrhythm/generator-boreas-env/commit/f4b099813c68c5707217ef5bf460cfec157684b9))

# [7.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.34.1...v7.0.0) (2020-09-03)


### Features

* update logrhythm-operator workload to make it compatible with kubernetes-base v0.47.1 ([a9abc07](https://github.com/logrhythm/generator-boreas-env/commit/a9abc07285e5895506b8cfd8a3204804fcdf919c))


### BREAKING CHANGES

* update to breaking change versions of kubernetes-base (v0.47.1) and logrhythm-operator (v0.10.0)

If you use logrhythm-operator in your cluster and use this version of the generator, you will need to use version v0.48.0+ of kubernetes-base and v0.10.0+ of logrhythm-operator (make sure your cluster is using imageTag v0.10.0 or higher for logrhythm-operator workload).

If you are not running logrhythm-operator workload in your cluster, this version doesn’t affect you.

## [6.34.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.34.0...v6.34.1) (2020-09-03)


### Bug Fixes

* adding sig processing to swagger options and fix semantic release ([6691939](https://github.com/logrhythm/generator-boreas-env/commit/66919394e34024e94f8f542b5c24b620fb7cc5e0))

# [6.34.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.33.0...v6.34.0) (2020-08-28)


### Features

* adding pgadmin workload ([94fcb19](https://github.com/logrhythm/generator-boreas-env/commit/94fcb19250a261b65dbd7f7a52044e4914912fd1))

# [6.33.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.32.2...v6.33.0) (2020-08-27)


### Features

* add a finalizer to all ArgoCD applications to instruct ArgoCD to cascadingly delete app’s resources on application delete ([107e0d9](https://github.com/logrhythm/generator-boreas-env/commit/107e0d90bec8a9cfbb5764d7b6bbf6052935c932))

## [6.32.2](https://github.com/logrhythm/generator-boreas-env/compare/v6.32.1...v6.32.2) (2020-08-26)


### Bug Fixes

* update SIEM UI runtime config and update some workload default configs ([66488f9](https://github.com/logrhythm/generator-boreas-env/commit/66488f9d332b3356af3e18577400ff50dcc87f84))

## [6.32.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.32.0...v6.32.1) (2020-08-26)


### Bug Fixes

* update default SIEM UI version match with new runtime config ([d6d62db](https://github.com/logrhythm/generator-boreas-env/commit/d6d62db6f72504c06dd9f6c4076a0d32c5deb9bc))
* update SIEM UI runtime config ([8123d9d](https://github.com/logrhythm/generator-boreas-env/commit/8123d9d2a0972587903ef03ccb0e1c4890238a89))

# [6.32.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.31.2...v6.32.0) (2020-08-25)


### Features

* **cluster:** add Unleash endpoint to Pomerium ([0d79b8d](https://github.com/logrhythm/generator-boreas-env/commit/0d79b8de613ab94cd9d1339a79c50ca4573ba243))
* **cluster:** update default version of logrhythm-operator ([deaafcd](https://github.com/logrhythm/generator-boreas-env/commit/deaafcd573534695dc04d60e919c99eeffd6e9e1))

## [6.31.2](https://github.com/logrhythm/generator-boreas-env/compare/v6.31.1...v6.31.2) (2020-08-24)


### Bug Fixes

* **quarkus:** Disable reactive-messaging healthchecks on services w/o Kafka ([faef1f5](https://github.com/logrhythm/generator-boreas-env/commit/faef1f5e7f2c130fe7740b6b3da1f62b1c273a62))

## [6.31.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.31.0...v6.31.1) (2020-08-24)


### Bug Fixes

* content-mgmt-svc and search-indexing-svc ([9cd8d48](https://github.com/logrhythm/generator-boreas-env/commit/9cd8d48a641adac55410938fcb0a68866c3fcbaa))

# [6.31.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.30.0...v6.31.0) (2020-08-24)


### Features

* **kops:** Upgrade to kops 1.18.0 and Kubernetes 1.18.8. REQUIRES MANUAL ROLLOUT ([907770e](https://github.com/logrhythm/generator-boreas-env/commit/907770ead0be1c4ce24c5ddbe9611793dd5d6af3))

# [6.30.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.29.0...v6.30.0) (2020-08-21)


### Features

* **pomerium:** Support pomerium v0.10.1 and enabling metrics ([eeb7b85](https://github.com/logrhythm/generator-boreas-env/commit/eeb7b8524ded0db462160d50941a18ce2b7f801c))

# [6.29.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.28.2...v6.29.0) (2020-08-20)


### Bug Fixes

* add back public key as in previous PR ([570729c](https://github.com/logrhythm/generator-boreas-env/commit/570729ca52c6d74507366e55e5b111b283cff6ff))
* remove some config items from app.properties and updated default image version for operator ([c8e52c6](https://github.com/logrhythm/generator-boreas-env/commit/c8e52c6009e708d36a55eac0a40faf8c0337bbf5))


### Features

* add search-indexing-svc workload ([c556af2](https://github.com/logrhythm/generator-boreas-env/commit/c556af275fc82a0107814d08726ac06d1c6c997f))

## [6.28.2](https://github.com/logrhythm/generator-boreas-env/compare/v6.28.1...v6.28.2) (2020-08-19)


### Bug Fixes

* Remove ACS-only config properties ([5621549](https://github.com/logrhythm/generator-boreas-env/commit/5621549606b0e4e0146845c7c8736cf1bdfce080))

## [6.28.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.28.0...v6.28.1) (2020-08-19)


### Bug Fixes

* **sshkey:** adjust initials key ([5f86623](https://github.com/logrhythm/generator-boreas-env/commit/5f866238c28fb134869726fe7b418d4fa8ace21c))

# [6.28.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.27.0...v6.28.0) (2020-08-19)


### Features

* **sshkey:** add bre's key ([ad7a623](https://github.com/logrhythm/generator-boreas-env/commit/ad7a6231c15867c45f93316ed209cb27e5a552bc))

# [6.27.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.26.1...v6.27.0) (2020-08-19)


### Features

* **auth-theme:** Support updated theme that requires runtime-config.js per environment ([50b62bb](https://github.com/logrhythm/generator-boreas-env/commit/50b62bb2fe7e31879932fbdda0e4aa851a1a80af))

## [6.26.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.26.0...v6.26.1) (2020-08-19)


### Bug Fixes

* content mgmt svc added to swagger ([9e5abe4](https://github.com/logrhythm/generator-boreas-env/commit/9e5abe436a8efce81fd301af9c5a204edc13a474))

# [6.26.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.25.0...v6.26.0) (2020-08-18)


### Features

* **keycloak:** Support auth-theme versioning in workload-config.json ([fbb3f9d](https://github.com/logrhythm/generator-boreas-env/commit/fbb3f9df16254a911c16228464cc60c4cdf1fcbf))

# [6.25.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.24.1...v6.25.0) (2020-08-18)


### Features

* **siem-ui:** Update configuration ([69f5d84](https://github.com/logrhythm/generator-boreas-env/commit/69f5d84f78b55edcda812a0e222f48a810fa1a8b))
* add content-mgmt-svc ([eb4836c](https://github.com/logrhythm/generator-boreas-env/commit/eb4836ca450b3366eda390859ef02bef9d6bfcc6))

## [6.24.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.24.0...v6.24.1) (2020-08-14)


### Bug Fixes

* Update .gitignore to ensure .idea files are ignored ([db9dbb0](https://github.com/logrhythm/generator-boreas-env/commit/db9dbb0be5db3adf1d5092298d2c75b98c4d6abd))

# [6.24.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.23.0...v6.24.0) (2020-08-14)


### Features

* **atlantis:** Add ecr directory to atlantis configuration ([b48885b](https://github.com/logrhythm/generator-boreas-env/commit/b48885b1501c601378364558b8af8b4b6b13a0b9))

# [6.23.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.22.0...v6.23.0) (2020-08-13)


### Features

* Add operations environment as supported for {file}.{env} overrides ([678ce22](https://github.com/logrhythm/generator-boreas-env/commit/678ce222bdb8cdcd1b832f9d7dd4cfedd90195aa))
* Operations environment uses different module versions ([113aadf](https://github.com/logrhythm/generator-boreas-env/commit/113aadf78c5693169d120bd5cd0c1d80e8bf52a0))

# [6.22.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.21.0...v6.22.0) (2020-08-13)


### Features

* Add Audit MFE ([1985c1d](https://github.com/logrhythm/generator-boreas-env/commit/1985c1d655150b4b9ddda9f422097cfd88bb8e49))

# [6.21.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.20.0...v6.21.0) (2020-08-13)


### Features

* **access-control-svc:** Add property introduced in https://github.com/logrhythm/boreas/pull/726 ([86e43f8](https://github.com/logrhythm/generator-boreas-env/commit/86e43f85977b0d8b6b8e0571218f46552bec1a74))
* **keycloak:** Allow username modifications in boreas realm ([0a56524](https://github.com/logrhythm/generator-boreas-env/commit/0a5652414fc3a088f9d0c5a79d46f6928e1300c7))

# [6.20.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.19.2...v6.20.0) (2020-08-13)


### Bug Fixes

* re-order of items in attempt to fix CI ([14c8cdb](https://github.com/logrhythm/generator-boreas-env/commit/14c8cdb4ea4f067e2429571df0ec83b4bf2d16e7))
* sort ordering causing linting to fail ([4a0377c](https://github.com/logrhythm/generator-boreas-env/commit/4a0377c2e794ce3afaa3bd4ce05050e83e8f3d71))
* syntax miss ([8f71844](https://github.com/logrhythm/generator-boreas-env/commit/8f7184414e7f057db7226fe3df965a6ecd73beac))
* units for mem ([1868e37](https://github.com/logrhythm/generator-boreas-env/commit/1868e379ce3304fe4439090d0b79d9322b347771))


### Features

* adding flink workload ([d3bbec9](https://github.com/logrhythm/generator-boreas-env/commit/d3bbec94ebdaafac184d5ca561f53a8c74d97062))

## [6.19.2](https://github.com/logrhythm/generator-boreas-env/compare/v6.19.1...v6.19.2) (2020-08-12)


### Bug Fixes

* **keycloak:** Set KEYCLOAK_FRONTEND_URL and fix scopes in Pomerium ([f0bf559](https://github.com/logrhythm/generator-boreas-env/commit/f0bf559162758765769ebc3f2c38ba8cf4bebf10))

## [6.19.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.19.0...v6.19.1) (2020-08-10)


### Bug Fixes

* **external-dns:** Hard-set v0.7.2. v0.7.3 does not work ([bb4a7c3](https://github.com/logrhythm/generator-boreas-env/commit/bb4a7c3a89fa2012242c3ffb227ef0af0a63fba5))

# [6.19.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.18.2...v6.19.0) (2020-08-06)


### Bug Fixes

* **ci:** change method of running environment check to make it `yo` independent ([60a7e8f](https://github.com/logrhythm/generator-boreas-env/commit/60a7e8f205350f872ef0d2acba10023706db420a))


### Features

* add an option to skip terraform/terragrunt runs ([f20178a](https://github.com/logrhythm/generator-boreas-env/commit/f20178afe6f92a563c4c813f899eb2e1bdcb1e1b))
* add environment up-to-date check ([9813997](https://github.com/logrhythm/generator-boreas-env/commit/98139978ef6c967989836312bffa72c1de5a960e))
* add MailHog workload to k8s cluster ([b41f41c](https://github.com/logrhythm/generator-boreas-env/commit/b41f41cb59c691a4be4d623cfe270b6844f78593))
* make SMTP credential optional in case it is not provided from terraform output ([d9af509](https://github.com/logrhythm/generator-boreas-env/commit/d9af50995ad594e26a5429f8dcea91abc903a1cf))

## [6.18.2](https://github.com/logrhythm/generator-boreas-env/compare/v6.18.1...v6.18.2) (2020-08-03)


### Bug Fixes

* Clarify current workload dependencies ([74c2992](https://github.com/logrhythm/generator-boreas-env/commit/74c2992d616cca27ad325d078bbe1e97efdae6af))

## [6.18.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.18.0...v6.18.1) (2020-07-31)


### Bug Fixes

* add missing issuer ([2e38fab](https://github.com/logrhythm/generator-boreas-env/commit/2e38fab940339e74f0c8082a78056b5d0b697bc9))

# [6.18.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.17.0...v6.18.0) (2020-07-30)


### Features

* **pomerium:** Enable Jaeger tracing ([84e6c9f](https://github.com/logrhythm/generator-boreas-env/commit/84e6c9ff6edb8aec76dd1985b6020ba3673d0f44))
* **pomerium:** Update pomerium helm chart to 11.0.0 ([6fea51a](https://github.com/logrhythm/generator-boreas-env/commit/6fea51a8dae08ce753a6a71d7b729298059ada03))

# [6.17.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.16.0...v6.17.0) (2020-07-30)


### Features

* enable audit-svc in acs and added kafka configs ([055cfe6](https://github.com/logrhythm/generator-boreas-env/commit/055cfe6aae630023b0ea9f5c8cdfe8b92ad952e9))

# [6.16.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.15.0...v6.16.0) (2020-07-30)


### Features

* **sonarqube:** Expose directly so that github auth can be used ([2f83f0c](https://github.com/logrhythm/generator-boreas-env/commit/2f83f0c88b5994a62d5fd98547429c76405213d0))

# [6.15.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.14.0...v6.15.0) (2020-07-29)


### Features

* dynamically configure pomerium workload ([7e58c69](https://github.com/logrhythm/generator-boreas-env/commit/7e58c69b9610e8a87d9e62d4bb0add73b98e2cd8))

# [6.14.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.13.1...v6.14.0) (2020-07-27)


### Features

* **sonarqube:** add namespace to internal url ([7200ed4](https://github.com/logrhythm/generator-boreas-env/commit/7200ed462ba96dbdfff071df525bc1c856de2f84))
* **sonarqube:** add sonarqube workload ([6f900a0](https://github.com/logrhythm/generator-boreas-env/commit/6f900a0bd5acf942aff42d3e944746be491bbfa8))
* **sonarqube:** remove infra true from workloads ([2908739](https://github.com/logrhythm/generator-boreas-env/commit/29087391db11e66a1a5cbaa4acfb1b265adc6fa8))

## [6.13.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.13.0...v6.13.1) (2020-07-27)


### Bug Fixes

* Update kafka bootstrap server name to contain namespace ([601d52a](https://github.com/logrhythm/generator-boreas-env/commit/601d52aa40df18a5016e2f988a906c7f4193e166))
* Update topic name in signal-ingest-svc configuration ([39b1719](https://github.com/logrhythm/generator-boreas-env/commit/39b17197c5e5be4939666d6b2952740cf2720c3e))

# [6.13.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.12.0...v6.13.0) (2020-07-27)


### Features

* deploy Auth and Siem-ui as MFEs ([8140e74](https://github.com/logrhythm/generator-boreas-env/commit/8140e74cbee531fb41599b463ad91cef44eb8398))

# [6.12.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.11.0...v6.12.0) (2020-07-24)


### Features

* add kafdrop kafka management ui to the generator ([074e96a](https://github.com/logrhythm/generator-boreas-env/commit/074e96a69ff8aa53b5e1b2d9b7f16d1fb74f9b64))

# [6.11.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.10.0...v6.11.0) (2020-07-21)


### Bug Fixes

* add audit-svc to  and add both new svcs to argo ([cacf818](https://github.com/logrhythm/generator-boreas-env/commit/cacf81886756442fac06ed8c7b83a32115ada5e6))
* remove trailing character from audit-svc.yaml ([f4071d7](https://github.com/logrhythm/generator-boreas-env/commit/f4071d7e834b15062fe44a0d2bf4200d41ba6a6f))
* signal-ingest template ([a281220](https://github.com/logrhythm/generator-boreas-env/commit/a281220b55795a2e8cbfaaaed02e9f25d79a80a4))


### Features

* **audit-svc:** add audit-svc templates ([0a56404](https://github.com/logrhythm/generator-boreas-env/commit/0a5640483aa28f5a3a8cb0837b8a843e84deb597))
* adding signal-ingest-svc ([5f7b0fd](https://github.com/logrhythm/generator-boreas-env/commit/5f7b0fd8edda8381877e4cb5abe6afa89c6292ba))

# [6.10.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.9.0...v6.10.0) (2020-07-21)


### Features

* add swagger-ui workload, dynamically generate swagger ui configs with dynamicProps ([88edac3](https://github.com/logrhythm/generator-boreas-env/commit/88edac3e74c3c752193cafbe0017aeb57cd37101))
* remember workload selection ([7cfce76](https://github.com/logrhythm/generator-boreas-env/commit/7cfce766d919920c348fc8f2f89dba049be145fc))
* **swagger-ui:** Add swagger-ui workload - WIP ([220a6d3](https://github.com/logrhythm/generator-boreas-env/commit/220a6d361ec6f4ffdcbc87c339ca0b8d7f4b5949))

# [6.9.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.8.0...v6.9.0) (2020-07-14)


### Features

* **kops:** Remove multi-master for personal sandboxes ([d7aff49](https://github.com/logrhythm/generator-boreas-env/commit/d7aff495f2d097c8cee6faec8a916bbc106ac839))

# [6.8.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.7.0...v6.8.0) (2020-07-14)


### Features

* embed AWS_PROFILE to kubeconfig ([b1da090](https://github.com/logrhythm/generator-boreas-env/commit/b1da09008a87696deeda5c6c2413f619352755c6))

# [6.7.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.6.0...v6.7.0) (2020-07-10)


### Features

* add ability to create kafka resources in lr-operator ([c068655](https://github.com/logrhythm/generator-boreas-env/commit/c0686551d3990b3ba945c0b4bf73371d3d1af35d))

# [6.6.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.5.0...v6.6.0) (2020-07-10)


### Features

* update default logrhythm-operator version to 0.2.0 ([a148f1a](https://github.com/logrhythm/generator-boreas-env/commit/a148f1ae531ddfdbf924bdb1726f48541e28359e))

# [6.5.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.4.0...v6.5.0) (2020-07-10)


### Features

* adding kafka cluster/topics/users workload as shared resource in an environment ([99a9815](https://github.com/logrhythm/generator-boreas-env/commit/99a9815d9a7565727b4b0e5b20db4d30da67bd41))

# [6.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.3.0...v6.4.0) (2020-07-09)


### Features

* **operations-cluster:** better comments, cleanup ([bd7511c](https://github.com/logrhythm/generator-boreas-env/commit/bd7511c6911486c6db07d1aac36b930b5a8ebbd2))
* **operations-cluster:** define workloadstoinstall var ([b6cbcc4](https://github.com/logrhythm/generator-boreas-env/commit/b6cbcc47879d5d76a86e54c0f24fa8001b16c691))
* **operations-cluster:** modify workload selection and add operations account ([9c12687](https://github.com/logrhythm/generator-boreas-env/commit/9c1268722afe68138808c9c6932a2febe8100788))
* **operations-cluster:** remove husky pre-commit ([8ba7b9a](https://github.com/logrhythm/generator-boreas-env/commit/8ba7b9ac9c1e3ac7c680de7453b90326b3949ed5))

# [6.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.2.0...v6.3.0) (2020-07-08)


### Features

* change ArgoCD instance label key ([434b08c](https://github.com/logrhythm/generator-boreas-env/commit/434b08cdab85713a671fc2f72f4d1848b5c4e113))

# [6.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.1.2...v6.2.0) (2020-07-01)


### Features

* save the generator version to environment config when run `yo boreas-env:cluster` ([4b93c39](https://github.com/logrhythm/generator-boreas-env/commit/4b93c3927b0fcc972ecb0fd5261c158f0b437d86))

## [6.1.2](https://github.com/logrhythm/generator-boreas-env/compare/v6.1.1...v6.1.2) (2020-07-01)


### Bug Fixes

* **prometheus:** Set correct externalUrl for alertmanager and prometheus ([509291a](https://github.com/logrhythm/generator-boreas-env/commit/509291a47a4d99b00a2dc6757a64bfbdd7ef901d))

## [6.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v6.1.0...v6.1.1) (2020-07-01)


### Bug Fixes

* correct ArgoCD wave value for some workloads ([4bf5589](https://github.com/logrhythm/generator-boreas-env/commit/4bf5589f93262e995d8324c8a058a16b6ce98e6e))
* improve waiting AWS IAM Authenticator mechanism ([c58e063](https://github.com/logrhythm/generator-boreas-env/commit/c58e06330bdea2fd5eeeae5c8de320897482476e))

# [6.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v6.0.0...v6.1.0) (2020-07-01)


### Bug Fixes

* **pomerium:** Add missing patches ([8ad674b](https://github.com/logrhythm/generator-boreas-env/commit/8ad674bf1ca5a9f680960d76c0886e20751bb4c9))
* **pomerium:** Refactor to fit new argocd applications structure ([968cf33](https://github.com/logrhythm/generator-boreas-env/commit/968cf33629341e790b1f163a5cb5173015df7d93))
* Ensure keycloak is always on a valid cert in personal sandboxes ([2054004](https://github.com/logrhythm/generator-boreas-env/commit/20540049b06aa4096dda6bbd1e8db711b2307374))
* **pomerium:** Add prompts for Pomerium vars ([c08c9a4](https://github.com/logrhythm/generator-boreas-env/commit/c08c9a4eb8e5aacd26d017341aa7061c5a6e2af4))
* **pomerium:** Fix test ([ea215f4](https://github.com/logrhythm/generator-boreas-env/commit/ea215f41ad72b56be4c6d2c23e6bb7069368f7d0))
* **pomerium:** Remove prompt validation for now and fix indentation ([65f899c](https://github.com/logrhythm/generator-boreas-env/commit/65f899c6edc03f9774835baf6891253d86798760))
* Add pomerium argocd application ([76c706d](https://github.com/logrhythm/generator-boreas-env/commit/76c706dab77098329d18843db5c79bdc5044cb87))
* Bring ACS and siem-ui up to date with Dev ([321b0fc](https://github.com/logrhythm/generator-boreas-env/commit/321b0fc55e69941f6c206f32100b058980c0a9b2))
* Comment loop lines for now ([0ea2416](https://github.com/logrhythm/generator-boreas-env/commit/0ea24168f3da53a7dd4942bd238b554db60ef455))


### Features

* **aws-iam-authenticator:** Remove aws-iam-patch due to kops 1.17.0 ([3af7209](https://github.com/logrhythm/generator-boreas-env/commit/3af7209741b4de114b61c93035b33c493da23ddc))
* **keycloak:** Add operations realm for pomerium ([f9e15ef](https://github.com/logrhythm/generator-boreas-env/commit/f9e15efa4e1b7514b5281da5401b0716ceb84c05))
* **pomerium:** Add Kiali and Jaeger proxying ([2526c08](https://github.com/logrhythm/generator-boreas-env/commit/2526c08089d2e5337232ed2d6008f2af05d72efe))
* **pomerium:** Add Pomerium workload ([8127c19](https://github.com/logrhythm/generator-boreas-env/commit/8127c19e6bb7fb00d6fff68aa03d11751ab0445e))
* **pomerium:** Add prometheus proxy ([607455b](https://github.com/logrhythm/generator-boreas-env/commit/607455b33cdd72e525ecb473efc5bf954cb7d859))
* **pomerium:** Enable grafana proxy thru pomerium ([11d36ed](https://github.com/logrhythm/generator-boreas-env/commit/11d36ed29fe22e14585040c4f7e9bbe9e88a661b))
* Add pomerium cluster-config.json vars ([26f535e](https://github.com/logrhythm/generator-boreas-env/commit/26f535e489eda7c42e8dd85aa410e9d5031f15f4))

# [6.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v5.0.1...v6.0.0) (2020-07-01)


### Features

* add istio (infra workload) ([6d0f5f2](https://github.com/logrhythm/generator-boreas-env/commit/6d0f5f246ebbf9c73302cd5e6874a99624350334))
* remove Rancher ([f8d4be3](https://github.com/logrhythm/generator-boreas-env/commit/f8d4be30b6d77f1f9cb0c187f22da61221aab94b))
* **grafana:** relocate grafana for new waves structure ([43a51d6](https://github.com/logrhythm/generator-boreas-env/commit/43a51d6cac32a0b5640930e5bfa15458cbbc8d16))
* add prometheus-operator (infra workload) ([498d6e7](https://github.com/logrhythm/generator-boreas-env/commit/498d6e7d9d400822f311b91d037829dad9d71e0e))
* update prometheus-operator ArgoCD waves ([dd917dd](https://github.com/logrhythm/generator-boreas-env/commit/dd917ddf8ae97832bbe0c2343c5213a4c2940e43))


### BREAKING CHANGES

* remove Rancher. Prometheus, Grafana, and Istio are now being managed by ArgoCD

You will need to destroy and rebuild your cluster, migration is not supported

## [5.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v5.0.0...v5.0.1) (2020-06-30)


### Bug Fixes

* remove hard-coded template files ([e461530](https://github.com/logrhythm/generator-boreas-env/commit/e46153061b4c555c3f409ecc6bbb2b035117f376))

# [5.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v4.4.0...v5.0.0) (2020-06-30)


### Features

* change cluster’s kubernetes workloads layout ([597f5d5](https://github.com/logrhythm/generator-boreas-env/commit/597f5d52c136dc8a649c915bd13a6847e9e8315b))


### BREAKING CHANGES

* change cluster’s kubernetes workloads layout to fix ArgoCD Waves

**Migration steps:**
- In your GitOps repo
- Run commands to clean up some unnecessary files
  ```zsh
  rm -rf vpc-01/clusters/*/kubernetes/argocd
  ```
- Rebuild your cluster with
  ```zsh
  yo boreas-env:cluster
  ```

# [4.4.0](https://github.com/logrhythm/generator-boreas-env/compare/v4.3.0...v4.4.0) (2020-06-23)


### Features

* adding kafka-operator workload to be managed by argoCD ([5468e2a](https://github.com/logrhythm/generator-boreas-env/commit/5468e2a5d5b3715488ea51850199b21c731dff98))

# [4.3.0](https://github.com/logrhythm/generator-boreas-env/compare/v4.2.0...v4.3.0) (2020-06-19)


### Features

* add aws-global/*.tf files to atlantis.yaml ([1e9b599](https://github.com/logrhythm/generator-boreas-env/commit/1e9b5991d45732385d5874b8b5dc807dc849ded2))

# [4.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v4.1.0...v4.2.0) (2020-06-17)


### Features

* **logrhythm-operator:** Update to v0.0.5 ([664e766](https://github.com/logrhythm/generator-boreas-env/commit/664e7668b8992a51bb0171a4193506ad9ea69df7))

# [4.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v4.0.2...v4.1.0) (2020-06-17)


### Features

* **logrhythm-operator:** Update image tag to v0.0.4 ([fde10ec](https://github.com/logrhythm/generator-boreas-env/commit/fde10ec5754df841404b546dda31774f1b9ffeee))

## [4.0.2](https://github.com/logrhythm/generator-boreas-env/compare/v4.0.1...v4.0.2) (2020-06-05)


### Bug Fixes

* corrected letsencryptIssuer to certIssuerName ([38be070](https://github.com/logrhythm/generator-boreas-env/commit/38be0706a56c212135f500bf18600ed6b73705ea))

## [4.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v4.0.0...v4.0.1) (2020-06-05)


### Bug Fixes

* cert issuer default and branching for personal sbxs fixed ([1e81eb7](https://github.com/logrhythm/generator-boreas-env/commit/1e81eb7c90df8bffef0d4e1d8097b4a986b4e510))

# [4.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v3.2.2...v4.0.0) (2020-06-04)


### Features

* migrate siem-ui to operator ([7ab77e2](https://github.com/logrhythm/generator-boreas-env/commit/7ab77e2c4e355679c3e896ab5dfcecd592b37b35))


### BREAKING CHANGES

* update siem-ui to use LogRhythm Operator and CR instead of workload descriptors

**Rollout steps for existing environments using previous Siem-Ui definition:**
- This migration is required for existing environments were deployed by the version `3.2.2` or older of the generator
- In the GitOps repo, remove `siem-ui` workload's descriptors excluding `workload-config.json` file:
    ```
    cp vpc-01/clusters/*/kubernetes/siem-ui/workload-config.json /tmp/workload-config.json
    rm -rf vpc-01/clusters/*/kubernetes/siem-ui/**
    cp /tmp/workload-config.json vpc-01/clusters/*/kubernetes/siem-ui
    ```
- Open your `siem-ui/workload-config.json`, if `imageTag` is `0.0.4-410` or older, update it to
    ```
      "imageTag": "0.0.4-497"
    ```
- Update the generator to this version and run:
    ```
    yo boreas-env:cluster-update --reconfig-workload
    ```
- Select submodule's ref that has `siem-ui` workload removed and `logrhythm-operator/siem-ui.crd.yaml` (currently in branch `add-siem-ui-operator`)
- Re-select workloads you want to deploy (all workloads should be selected by default)
- Verify changes in your GitOps repo locally but **DON'T DEPLOY/PUSH THE CHANGES YET**:
  - You should see a bunch of files of siem-ui is deleted
  - You should see siem-ui is being deployed using the CR.
- Go to ArgoCD: click on **Delete** on `siem-ui` panel -> Leave "Cascade" selected -> Click on "Ok" (you might need to delete it twice if it re-appears right away)
- **Wait for `siem-ui` panel to be disappeared**, and `argo-cd` panel will display `missing` and `out-of-sync`, but that's expected
- Deploy the changes to the environment (open a PR or push to master if personal sandbox)
- Go to ArgoCD and click on "Refresh" on `argo-cd` panel
- Watch ArgoCD:
  - Siem-ui panel should show out of sync and missing (this is expected because it can be synced only after LogRhythm Operator is deployed) - Now Click on **Sync** on `siem-ui` panel.
  - siem-ui should be updated to use the CR
- After giving some time for the route53 records to be recreated you can do smoke test for Siem-ui : https://confluence.logrhythm.com/display/NGP/Smoke+Tests

## [3.2.2](https://github.com/logrhythm/generator-boreas-env/compare/v3.2.1...v3.2.2) (2020-06-03)


### Bug Fixes

* **access-control-svc:** Update config per https://github.com/logrhythm/boreas/pull/440 ([585a483](https://github.com/logrhythm/generator-boreas-env/commit/585a483be9ce8bb9a6c9a30d1d83f9172cbcb80e))

## [3.2.1](https://github.com/logrhythm/generator-boreas-env/compare/v3.2.0...v3.2.1) (2020-06-02)


### Bug Fixes

* **access-control-svc:** Correct jwt key config and set jwt issuer ([e734fd9](https://github.com/logrhythm/generator-boreas-env/commit/e734fd9ee99ef393696da4bad016915ed7b65be3))

# [3.2.0](https://github.com/logrhythm/generator-boreas-env/compare/v3.1.0...v3.2.0) (2020-06-01)


### Features

* **loki:** add loki ([f9c3660](https://github.com/logrhythm/generator-boreas-env/commit/f9c366001059e442d5b7359e5d9694778733200a))

# [3.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v3.0.0...v3.1.0) (2020-06-01)


### Features

* **cluster-update:** save generator version to environment-config.json ([fa188f1](https://github.com/logrhythm/generator-boreas-env/commit/fa188f1fcda1e09140b45f9e1ebf46f67f50627c))

# [3.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v2.1.2...v3.0.0) (2020-06-01)


### Bug Fixes

* make ACS dependent of logrhythm-operator ([14e98e4](https://github.com/logrhythm/generator-boreas-env/commit/14e98e4e5c6a32c362abde0c0d9b6ec2fe92ae09))
* remove incorrect config from access-control-svc CR ([a6acb15](https://github.com/logrhythm/generator-boreas-env/commit/a6acb15ae28f47fed0238ccde2b5481e18fb448d))


### Features

* add logrhythm-operator workload ([e7f1381](https://github.com/logrhythm/generator-boreas-env/commit/e7f13812a5fcc26f6dfd694fa3b019f87e179667))
* change access-control-svc deployment descriptors ([42ccfaf](https://github.com/logrhythm/generator-boreas-env/commit/42ccfafb0bd7b62138c9b03d9cb07d4bbecb1ebd)), closes [/github.com/logrhythm/boreas-kubernetes/pull/76/files#diff-960891c8c8514160120315226402799](https://github.com//github.com/logrhythm/boreas-kubernetes/pull/76/files/issues/diff-960891c8c8514160120315226402799)


### BREAKING CHANGES

* update access-control-svc workload to use LogRhythm Operator instead of raw descriptors

**Rollout steps for existing environments using previous ACS definition:**
- This migration is required for existing environments were deployed by the version `2.1.2` or older of the generator
- In the GitOps repo, remove `access-control-svc` workload's descriptors excluding `workload-config.json` file:
    ```
    cp vpc-01/clusters/*/kubernetes/access-control-svc/workload-config.json /tmp/workload-config.json
    rm -rf vpc-01/clusters/*/kubernetes/access-control-svc/**
    cp /tmp/workload-config.json vpc-01/clusters/*/kubernetes/access-control-svc
    ```
- Open your `access-control-svc/workload-config.json`, if `imageTag` is older than `20200518170420-228d61b-20200518171316`, update it to
    ```
      "imageTag": "20200518170420-228d61b-20200518171316"
    ```
- Update the generator to this version and run:
    ```
    yo boreas-env:cluster-update --reconfig-workload
    ```
- Select submodule's ref that has `logrhythm-operator` workload added
- Re-select workloads you want to deploy (all workloads should be selected by default)
- Verify changes in your GitOps repo locally but **DON'T DEPLOY/PUSH THE CHANGES YET**:
  - You should see `logrhythm-operator` workload is added
  - You should see a bunch of files of ACS is deleted
  - You should see ACS is being deployed using LogRhythmService CR.
- Go to ArgoCD: click on **Delete** on `access-control-svc` panel -> Leave "Cascade" selected -> Click on "Ok" (you might need to delete it twice if it re-appears right away)
- **Wait for `access-control-svc` panel to be disappeared**, and `argo-cd` panel will display `missing` and `out-of-sync`, but that's expected
![image](https://user-images.githubusercontent.com/10015525/83279259-17834f00-a192-11ea-8f51-c81433ffe7b4.png)
- Deploy the changes to the environment (open a PR or push to master if personal sandbox)
- Go to ArgoCD and click on "Refresh" on `argo-cd` panel
- Watch ArgoCD:
  - LogRhythm Operator workload should be deployed and healthy
    <img width="468" alt="Screen Shot 2020-05-28 at 4 10 10 PM" src="https://user-images.githubusercontent.com/10015525/83201253-523da680-a102-11ea-812d-ad83edd65dca.png">
  - ACS panel should show out of sync and missing (this is expected because it can be synced only after LogRhythm Operator is deployed) - Now Click on **Sync** on `access-control-svc` panel.
  - ACS should be updated to use LogRhythmService CR
    <img width="1665" alt="   " src="https://user-images.githubusercontent.com/10015525/83201320-7b5e3700-a102-11ea-830e-92c1ffc47682.png">

## [2.1.2](https://github.com/logrhythm/generator-boreas-env/compare/v2.1.1...v2.1.2) (2020-05-26)


### Bug Fixes

* **cluster-update:** submodule version selector - correct tags order ([6b48aa5](https://github.com/logrhythm/generator-boreas-env/commit/6b48aa59d18f8ac21d1ca0cb6f71aaed40ff1bde))

## [2.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v2.1.0...v2.1.1) (2020-05-21)


### Bug Fixes

* missing pieces of renaming production to prod ([71142d1](https://github.com/logrhythm/generator-boreas-env/commit/71142d1c8a77bf6e6d07451abfe69acb97a9d657))

# [2.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v2.0.2...v2.1.0) (2020-05-20)


### Features

* change production to prod ([428826d](https://github.com/logrhythm/generator-boreas-env/commit/428826df975e17d305f4517a6d96f3a0cf790b7c))

## [2.0.2](https://github.com/logrhythm/generator-boreas-env/compare/v2.0.1...v2.0.2) (2020-05-18)


### Bug Fixes

* **ci:** semantic-release broken because of @ char ([b9401c6](https://github.com/logrhythm/generator-boreas-env/commit/b9401c6b8e110e3f53da5c4bac84069db8248017))

## [2.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v2.0.0...v2.0.1) (2020-05-15)


### Bug Fixes

* **siem-ui:** Correct runtime config from boreas PR[#382](https://github.com/logrhythm/generator-boreas-env/issues/382) ([be8f8e4](https://github.com/logrhythm/generator-boreas-env/commit/be8f8e43b883a99e43a4760d40b7533031fa3255))

# [2.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v1.2.1...v2.0.0) (2020-05-15)


### Features

* **keycloak:** Update realm and related workloads ACS and SIEM-UI ([a277912](https://github.com/logrhythm/generator-boreas-env/commit/a277912524244cbb061445a3c34ffa1fe17cb45a))


### BREAKING CHANGES

* **keycloak:** Update Keycloak realm

**Rollout steps for existing environments using previous realm definition:**
- Update access-control-svc version
  ```
  WORKLOAD=access-control-svc
  IMAGE=20200515160124-a27ad9e-20200515160818
  CLUSTER=k8s
  VPC=vpc-01
  WORKLOAD_CONFIG=${VPC}/clusters/${CLUSTER}/kubernetes/${WORKLOAD}/workload-config.json
  jq '.imageTag = "'${IMAGE}'"' ${WORKLOAD_CONFIG} > ${WORKLOAD_CONFIG}.new
  mv ${WORKLOAD_CONFIG}.new ${WORKLOAD_CONFIG}
  ```
- Update siem-ui version
  ```
  WORKLOAD=siem-ui
  IMAGE=0.0.4-410
  CLUSTER=k8s
  VPC=vpc-01
  WORKLOAD_CONFIG=${VPC}/clusters/${CLUSTER}/kubernetes/${WORKLOAD}/workload-config.json
  jq '.imageTag = "'${IMAGE}'"' ${WORKLOAD_CONFIG} > ${WORKLOAD_CONFIG}.new
  mv ${WORKLOAD_CONFIG}.new ${WORKLOAD_CONFIG}
  ```
- Update cluster definition
  - `yo boreas-env:cluster-update`
- Deploy this change to the environment
- Wait for ArgoCD to sync keycloak application, resulting in the "realms" configmap being updated
- Log into Keycloak (https://idp.{cluster-domain}) as "keycloak" user
- Delete "Boreas" realm
- Terminate keycloak pod, which will cause Keycloak to create the Boreas realm based off the configmap `kubectl delete pod -n keycloak lr-keycloak-0`

## [1.2.1](https://github.com/logrhythm/generator-boreas-env/compare/v1.2.0...v1.2.1) (2020-05-15)


### Reverts

* "chore(release): 1.2.0 [skip ci]" ([f3e5c2a](https://github.com/logrhythm/generator-boreas-env/commit/f3e5c2ad491935e920e71379e9c58f5df9ef2ac2))
* "Merge pull request [#62](https://github.com/logrhythm/generator-boreas-env/issues/62) from logrhythm/US7017-keycloak-realm-update" ([bc46ea9](https://github.com/logrhythm/generator-boreas-env/commit/bc46ea94a4b9730722e5f99fb1345ddfc02c3a9a))

# [1.1.0](https://github.com/logrhythm/generator-boreas-env/compare/v1.0.2...v1.1.0) (2020-05-15)


### Features

* **app:** update atlantis workflow to save cluster TF output ([54b15de](https://github.com/logrhythm/generator-boreas-env/commit/54b15de22f5a05249cf6ecb5fb54b4a4a741df20))

## [1.0.2](https://github.com/logrhythm/generator-boreas-env/compare/v1.0.1...v1.0.2) (2020-05-15)


### Bug Fixes

* **cluster-update:** remove AWS environment check as this generator doesn’t mutate environment ([ceed7bf](https://github.com/logrhythm/generator-boreas-env/commit/ceed7bf46f8a723c8135aea7d91a91a450e13f55))

## [1.0.1](https://github.com/logrhythm/generator-boreas-env/compare/v1.0.0...v1.0.1) (2020-05-15)


### Bug Fixes

* --fix-cluster-infra didn't save the new tf output ([913148c](https://github.com/logrhythm/generator-boreas-env/commit/913148c053db652ad15fddf93284bcfb31ad14c6))

# [1.0.0](https://github.com/logrhythm/generator-boreas-env/compare/v0.2.1...v1.0.0) (2020-05-14)


### Bug Fixes

* **cluster-update:** cluster.json is not saved ([b994483](https://github.com/logrhythm/generator-boreas-env/commit/b994483bc422988a165d529e9e676639083ac693))


### Features

* make the generator single source of truth for all environments ([79efb5c](https://github.com/logrhythm/generator-boreas-env/commit/79efb5c3429a4aa5043d34713f995a509d3f1317))


### BREAKING CHANGES

* new environment configuration layouts

**Migration steps for environments generated using older version of the generator:**
- Update the generator with this PR changes (don't forget `npm install`)
- In an environment GitOps repo:
```zsh
CLUSTER_SHORT_NAME=k8s # change this

cat .yo-rc.json | jq -r '."generator-boreas-env" | { personal_sandbox,aws_account_id,environment,namespace,vpc_dir_name,cidr,cluster_short_name,kubernetes_base_ref,generator_version }' > environment-config.json
cat .yo-rc.json | jq -r '."generator-boreas-env" | {gitops_repo_https}' > vpc-01/clusters/$CLUSTER_SHORT_NAME/cluster-config.json

rm .yo-rc.json
yo boreas-env
```
- You should see a new file generated in your cluster dir which is terraform output of kops
```zsh
cat vpc-01/clusters/$CLUSTER_SHORT_NAME/zz_generated.tf_output.json
```
- Run following commands to update cluster configuration
```zsh
yo boreas-env:cluster-update --reconfig-workload
```
- Follow the prompt, commit and push all changes (will need to open a PR for boreas-env-* environment)

**CHANGE DETAILS:**

**main**:
1. Now write environment configuration to `environment-config.json` in the root of the gitops repo including the current version of the generator
2. Write terraform output for kops to `zz_generated.tf_output.json` in cluster dir, which will be consumed by downstream generators

**cluster**:
1. Now allow users to choose which workloads to deploy to the cluster
2. Available workloads are defined in `generators/cluster/workload.js` **<= adding a new workload now requires modifying this file**
3. Write cluster configuration to `cluster-config.json` in cluster dir
4. Generate `workload-config.json` for workloads having defaultWorkloadConfig defined in `workload.js`
5. Add option `--reconfig-workload`

**cluster-update**:
1. Support CI workflow by providing `--ci` to `yo boreas-env:cluster-update` command:
    - No prompts at all
    - Read configuration from the environment to populate workload files
    - Force overriding all files
2. Add option `--reconfig-workload`
3. Add option `--use-default-workload-config`

For more information: https://github.com/logrhythm/generator-boreas-env/pull/58

## [0.2.1](https://github.com/logrhythm/generator-boreas-env/compare/v0.2.0...v0.2.1) (2020-05-14)


### Reverts

* "chore(release): 0.2.0 [skip ci]" ([457dea6](https://github.com/logrhythm/generator-boreas-env/commit/457dea63ea771899b9fd1a1fafd32d424c32be0f))
* "Merge pull request [#55](https://github.com/logrhythm/generator-boreas-env/issues/55) from logrhythm/single_source_of_truth" ([34a949b](https://github.com/logrhythm/generator-boreas-env/commit/34a949b62b9e15eb21410ec15e35ca97ff29b3f1))

## [0.1.2](https://github.com/logrhythm/generator-boreas-env/compare/v0.1.1...v0.1.2) (2020-05-13)


### Bug Fixes

* compress resulting userdata block ([2095873](https://github.com/logrhythm/generator-boreas-env/commit/20958735b60b1a45b79289523c9601caaa238316))

## [0.1.1](https://github.com/logrhythm/generator-boreas-env/compare/v0.1.0...v0.1.1) (2020-05-12)


### Bug Fixes

* adding changelog to semantic-release ([2bb0f0e](https://github.com/logrhythm/generator-boreas-env/commit/2bb0f0e93038d26091b409a892c534d7abd02d23))
