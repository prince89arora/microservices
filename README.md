# microservices

## Benefits

- Effective smaller team with single context to focus on single responsibility. Manageable smaller teams.
- Smaller codebase to manage makes it easier to ship and test. Smaller items to test and with better results quality.
- Different techs can be used easily for different services. No tech stack limitations. Its possible to use a different tech stack for a module of application depending on the load and type of work it does.
- Easy test automation to reduce testing cycle time.
- Scaling and descaling is easier and can scale individual part of appliance in this case service. Less expensive.
- Easy to keep different services secure an issue or 3rd party library can only affect 1 microservice.

## Challenges

- Network communication between modules/services. Services should be designed to minimize network latency. To reduce the network calls and provide data with minimum calls. Avoid chatty behavior.
- Complex network scenarios to handle. Since state and data is distributed, need additional sophisticated failure handling approach. Need to have solutions depending on type of network issues. Example: Retry cannot be a solution when computation is an issue for a service.
- Cascading failure, the type of failures that are happening because of other dependencies on the main service like API gateway failure.
- Amplification Effects
- Downtime and outage
- Logging and debugging is harder in microservices since the flow is involving different microservices and distributed state. Observability is crucial.
- Need to have robust automation like Tests, deployment, Monitoring and scaling.
