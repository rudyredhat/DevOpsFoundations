# Infrastructure Automation
## `Infra as code: IaC`
  - Dev, Staging & Production env must be visible
  - Codes must be managed by SCM
  - Put in SC, run in pipeline and then test it
`--------------------------------------------------------------------------------------------------------`
## `Configuration Management`
  - Heart of infra automation
  - Steps
    - Provisioning
    - Deployment
    - Orchestration
    - Configuration Management
  - How tools approach configuration management ?
    - Imperative (Procdeural)
    - Declarative (Functional)
    - Idempotent
    - Self-Service
`--------------------------------------------------------------------------------------------------------`
## `Immutable Deployment`
  - Why using diff models for diff phase?
    - The container pipeline can be the ans, where servers are being packed in the container
  - CMDB = configuration management database, dataware house containing info of all IT assets
`--------------------------------------------------------------------------------------------------------`
## `Infra toolchain`
  - depends on the back-end used
  - CM
    - chef
    - puppet
    - ansible
    - salt
    - cfengine
    - packer
  - service directory tools
    - etcd
    - zookeepre
    - consul
  - orchestration of containers 
    - docker swram
    - kubernetes
    - mesos
