# DevOps Practices
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
