# Reliability Engineering
## `Engineering does not end with deployment`
  - Reliability = ability of a sys or component to function under stated conditions for a specified period of time
  - MTTR = mean time to recovery, how quickly a service can recover from a disruption and restore service
  - MTBF = mean time between failures, avg time between service disruptions
  - eg = SRE 
  
`-------------------------------------------------------------------------------------------`
## `Operation: Theory, Practice , Design (Metrics & Monitoring)`
  - **[Book- Release It!](https://www.oreilly.com/library/view/release-it/9781680500264/)**
  - Cascading failures can be overcome by the Circuit Breaker pattern
  - app for service ready deployment [blog](https://12factor.net/)
  - [Netflix chaos monkey](https://github.com/Netflix/chaosmonkey)
    - kill unwanted servers
  - [How complex system fails](https://www.he-alert.org/filemanager/root/site_assets/standalone_pdfs_0355-/HE00545.pdf)
  - 6 areas of monitoring
    - service perf and uptime
    - soft component metrics
    - system metrics
    - app metrics
    - performance
    - security
    
`-------------------------------------------------------------------------------------------`
## `Logging`
  - used by devs and ops teams
  - five Ws of logging?
    - what happend?
    - when did it happen?
    - where did it happen?
    - who was involved?
    - where did that entity come from?
`-------------------------------------------------------------------------------------------`
## `SRE toolchain`
  - saas monitoring
    - pingdom, datadog, netuitive, ruxit, librato, new relic, appdynamics
  - open-source monitoring
    - statsD, ganglia, graphite, grafana
    
