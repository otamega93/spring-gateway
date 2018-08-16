# spring-gateway
Spring gateway PoC

This gateway microservice consumes the reactive-account microservice. It maps the url and uses load balancing (internally Ribbon) to balance and then forward to the actual microservice.

Url to consume the reactive-account MS: http://localhost:8081/accounts/** (it replaces the /account/ segments of the url, get the next segment or segments of the url and then use that segments to make the new path to forward the requests).
