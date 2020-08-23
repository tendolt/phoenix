# Phoenix

A task to evaluate development skills.

### Service description

Service which is always-on. Demonstrate an ability to design and develop 
a resilient service able to withstand DDOS attacks. 
This should be a simulation and not actual resilient distributed service.

### Service specification

 - There should be at least 1 service instance alive and able to serve a service at any given moment
 - In front of service instances sits load balancer which routes client traffic to service instances
 - If service instance receives more than 10 requests per sec. - consider such an instance overloaded and spawn a new instance
 - For the sake of simplicity assume that load-balancer does not get overloaded
 - If consumer traffic reduces - shutdown not needed service instances to save resources
 - Clients generate huge traffic randomly (DDOS simulation) overloading the service
 - Processing client request takes some random time
 - Service instance should process request within pre-defined time otherwise consider request failed

### Service visualisation

  - Print out currently active service instances and how many requests are being process by them
  - Print out average request processing rate by any given service instance
  - Print out total processed / failed requests by any given instance
  - Print out total routed / failed requests by load-balancer

### Requirements

 - Fulfill specification - implementation should follow service specification given
 - Language agnostic - choose your own language. Bonus for using golang
 - Concentration - try to fit in 1 working day, focus on requirements
 - Clean code - demonstrate concise and readable code
 - Design patterns - demonstrate your design skills (SOLID, KISS, DRY etc.)
 - Testing - demonstrate testing skills by writing tests for your solution
 - Verifiable - we should be able to launch your solution with ease
 - Share your code on github and send us a link to info@tendo.lt
