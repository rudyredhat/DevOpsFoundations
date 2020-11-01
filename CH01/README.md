# DevOps
## `DevOps ?`
- Practice of `operations` and `development engineers` participating together in the entire service lifecycle.
  - **DESIGN** `-->` **DEVELOPMENT** `-->` **PRODUCTION** = `CODE`+`TEST`+`DEPLOY`+`OPERATE`
  - Can be break down to `5` levels:
    - Values
    - Principles
    - Methods
    - Practices
    - Tools
  - Why Devops ?
    - Faster outcomes
    - Making day to day life easier
  - What is `Dev` + `Ops` ?
    - `Development` = Developers + Front end + QA
    - `Operations` = System, Network, DB (admins)

## `DevOps Values`
- CAMS
  - About **[CAMS Model](https://blog.chef.io/what-devops-means-to-me/)**
    - `Culture` + `Automation` + `Measurement` + `Sharing`
  - [God father](https://twitter.com/patrickdebois?s=20) of Devops
  - `Culture` is about removing the barrier between Dev & Ops
  - `Automation` we have people > process > tools
  - `Measurement` is about the
    - Mean time to recovery
    - Cycle time
    - Cost
    - Revenue
    - Employee Satisfaction
  - `Sharing` is generally heart of DevOps

## `DevOps Principles`
- The Three ways Principles: [Gene Kim](https://itrevolution.com/the-three-ways-principles-underpinning-devops/)
  - Principles were:
    - `Systems thinking`
      - Focus on the overall outcome of the entire pipeline or value chain
      - From Concept to Cash:
        - If all your codes is not properly deliver to the customer then we loose it
    - `Amplyfying Feedback loops`
      - Creating Shortening and amplifying feedback loops
      - For eg: If a `bug` is raised, it must a process workflow in each stage, otherwise it may get released without tested.
    - `Culture of Continous experimentation and learning`
      - Open to learn new things and actively tries how it works or not
      - Master the skills with the repition of practice
      - e.g = `If it hurts, do it more`

## `DevOps Methodologies`
- Five most prevalent methodologies
  - First Methodology
    - `People over Process over Tools` by [Alex Honor](http://dev2ops.org/2010/02/people-over-process-over-tools/)
  - Second Methodology
    - `CD` = Code, Test & Release Software frequently
      - eg = [DevOps Transformation](https://itrevolution.com/the-amazing-devops-transformation-of-the-hp-laserjet-firmware-team-gary-gruver/)
  - Third Methodology
    - `Lean Management`
      - work in small batches
      - work in progress limits
      - feedback loops
  - Fourth Methodology
    - `The Visible OPS Style Change Control` = [Book](https://www.amazon.com/Visible-Ops-Handbook-Implementing-Practical/dp/0975568612)
    - Direct coleration between operational success and control over changes in env
      - Eliminate fragile artifacts
      - Create a repeatable build process
      - Manage Dependencies
  - Fifth Methodology
    - `Infrastructure as Code`
      - System treated like code
      - Checked into source control
      - Reviewed, built and tested

## `DevOps Practices`
  - 10. `Incident Command System` - All the bad things happens to the IT, called as Incidents
  - 9. `Developers on Call` - Fast feedback loop, with mogging and deployment, application problem is resolved quickly
  - 8. `Public Status Pages` - Through communication we can achieve uptime. **[Blog](http://www.transparentuptime.com/)**
  - 7. `Blameless Postmortems` - Single root cause or human error for failures. **[Blog](https://codeascraft.com/2012/05/22/blameless-postmortems/)**
  - 6. `Embedded Teams` - If dev teams want to new code and ops team wants to have service up, inside that there is inherent conflict of interest, so teams allow to have operations engineers and work accordingly.
  - 5. `The Cloud` - Giving you API-driven way to create and control infrastructure.
  - 4. `Andon Cords`- Releasing quickly, but there are automation tests which aren't perfect. Used by Toyata, is same as a hanging wire/cord in the bus in which anyone can pull the cord if having any problem. In the same way we can have this in software delivery pipeline.
  - 3. `Dependency Injection` - Database, rest APIs are possibly the runtime issues, so there are software pattern called dependency injection or inversion of control which focus on loosely coupled dependency. **[Blog](https://martinfowler.com/articles/injection.html)**
  - 2. `Blue-Green Deployment` - Take down the software, upgarde it and bring it back up. SO instead of testing a release in a staging env and deploying it to production env and hoping it works, instead we have two identical systems , blue & green, where blue(live). Where we are shifting the traffic from blue to green.
   ```
     Load Balancer
            |
      _______________
     |               |
   Blue           Green
   ```
   - 1. `Chaos Monkey` - In old style sys - making each component of a sys available to achieve the highest available uptime. But now there is chaos monkey, used by `netflix` on amazon cloud , which kills the server which forces operators and devs creating the systems to engineers resiliency into their services instead of thinking that infra is always on.

## `DevOps Tools`
  - Use for code, build, test, package, release, configure, monitor sys and appln.
  - So we have series of tools that can be converted to tool chain. **[Blog](https://en.wikipedia.org/wiki/DevOps_toolchain)**
  - we need to focus on following:
    - Tool criteria
      - Programmable - invoke from API or call from cmd line.
      - Verifiable - events and metrics are the imp feedback.
      - Well behaved - use for source control, test would verify the behaviour and able to deploy it in automated manner.
