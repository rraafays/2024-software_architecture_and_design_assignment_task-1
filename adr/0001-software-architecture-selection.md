---
parent: Decisions
nav_order: 100
title: Decide on Architecture

# status: accepted
# date: 2024-10-01
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Software Architecture

## Context and Problem Statement

AML would like to commission a new system which enables users to search, borrow and return media seamlessly regardless of location as well as allow for a 10% growth in user base annually. This record is to decide what architecture the new system should follow to ensure it can meet these goals.

Currently, AML uses a legacy CMS system which is evident in the case study. This legacy CMS system is a limiting factor for AML. Switching to a headless CMS provides AML with far more options as well as ensuring that they have access to an admin panel without needing to create one from scratch.

## Considered Options

* Client-Server
* Monolithic
* Microservices

## Decision Outcome

Chosen option: Client-Server, because it allows for all the features that AML require to be implemented and used seamlessly online by Library Members, but it also allows for further expansion which accounts for the annual growth of 10% in user base. Additionally, each client can differ which may allow AML to expand their services in the future

### Consequences

* Good, because it appears to align with the goals AML has when envisioning this new system, and it also allows for future expansion if necessary.

### Confirmation

This ADR will be confirmed by the success of the system we are architecting for AML as the architecture is core to the implementation of the system.

## More Information

As a development team we are very experienced with the Client-Server architecture which will make development much more streamlined.

### References

Berson, A. (1996). Client/server architecture. McGraw-Hill, Inc..
De Lauretis, L. (2019, October). From monolithic architecture to microservices architecture. In 2019 IEEE International Symposium on Software Reliability Engineering Workshops (ISSREW) (pp. 93-96). IEEE.
Cerny, T., Donahoo, M. J., & Trnka, M. (2018). Contextual understanding of microservice architecture: current and future directions. ACM SIGAPP Applied Computing Review, 17(4), 29-45.
