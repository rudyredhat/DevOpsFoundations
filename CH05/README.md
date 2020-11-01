# Continuous Delivery
## `Small+Fast = Better`
  - Unit test are run and appln is deployed into a prod like env
  - code is always in working state in CD
  - `CI` = automatically building and unit testing the entire appln
  - `CDelivery` = deploying every change to a production like env and performing automated integration and acceptance testing
  - `CDeploy` = after testing every change, automatically deploying to prod

## `CI practices`
  - `CD` = code -> build -> unit tests -> code validation -> packaging -> artifact
  - CI practice
    - all builds pass the coffee test (less than 5 min)
    - commit really small bits
    - don't leave a build broken
    - use a trunk-based development flow
      - no long running branches
      - multiple commits each day
    - don't allow flaky test, fix them
    - the build should return a status, a log and an artifact

## `CDelivery pipelines`
  - Only build arifacts once
  - artifacts should be immutable
  - flow of artifacts
    - code -> VC -> CI system creates build -> artifact added to central repo -> staging -> testing -> ready for production
  - staging should be a copy of prod
  - stop deploy if a previous step fails
  - deployments should be idempotent

## `QA role`
  - types of testing
    - unit testing
    - code hygiene
    - integration testing
    - TDD (test driven development) , BDD (behavior DD), ATDD (acceptance TDD)
    - infra testing
    - performance testing
    - security testing
    
## `CI toolchain`
  - six phases
    - VC
      - commit code changes, git , butbucket
    - CI systems
      - jenkins
    - Build
      - workflow approach using maevan
    - Test
    - Artifact repo
      - docker hub, amazon s3
    - Deployment
