---
parent: Decisions
nav_order: 100
title: Testing Strategy & Framework

# status: accepted
# date: 2024-10-01
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Testing Strategy & Framework

## Context and Problem Statement

There is a lack of clarity on whether AML's legacy system ever implemented unit testing methodologies. This absence of documentation or evidence of prior testing creates uncertainty around the testing culture and practices of the legacy system. Without this foundational knowledge, the development team faces potential difficulties in ensuring the reliability and maintainability of the new system, as they cannot draw insights or lessons from past testing strategies.

## Considered Options

* Jest
* Supertest
* SQLite3 with In-Memory Databases

## Decision Outcome

Chosen options: Jest, Supertest, SQLite. Jest will serve as our primary testing library due to its robust feature set and ease of use. Supertest will be employed for API endpoint testing. SQLite will be used as our in-memory database during testing to ensure lightweight and efficient data handling.

### Consequences

* Good, hhis combination provides a comprehensive and flexible approach to testing, ensuring that our codebase remains reliable and maintainable.

### Confirmation

The success of our testing strategy and framework will be demonstrated through high test coverage, successful integration and E2E tests with Supertest, performance benchmarks using SQLite, seamless CI/CD pipeline integration with Jest, positive developer feedback on test usability, and a reduction in production bugs, allowing us to confidently assess their impact.

## More Information

It is best to complement SQLite tests with integration tests against the actual database system used in production to ensure higher fidelity and confidence in the application's robustness and performance.

### References

Park, J., An, S., Youn, D., Kim, G., & Ryu, S. (2021, May). Jest: N+ 1-version differential testing of both javascript engines and specification. In 2021 IEEE/ACM 43rd International Conference on Software Engineering (ICSE) (pp. 13-24). IEEE.
Sasikumar, S., Prabha, S., & Mohan, C. (2022, May). Improving performance of next. js app and testing it while building a badminton based web app. In Proceedings of the International Conference on Innovative Computing & Communication (ICICC).
Artzi, S., Dolby, J., Jensen, S. H., Møller, A., & Tip, F. (2011, May). A framework for automated testing of JavaScript web applications. In Proceedings of the 33rd International Conference on Software Engineering (pp. 571-580).
