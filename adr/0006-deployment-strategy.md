---
parent: Decisions
nav_order: 100
title: Deployment Strategy

# status: accepted
# date: 2024-10-01
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Deployment Strategy

## Context and Problem Statement

In transitioning to a new system, one of the key challenges is ensuring user adoption and retention. Without a strategic deployment plan, users may face difficulties adapting to new interfaces and functionalities. By focusing on user-centric deployment, we can mitigate resistance to change and foster long-term retention.

## Considered Options
When considering deployment strategies, it is important to evaluate the goals and constraints of the deployment process. Several common deployment strategies can be considered:

1. **Rolling Deployment**: This strategy involves gradually replacing instances of the application with the new version. It allows for zero downtime and rollback if issues arise. However, it may require additional infrastructure to run multiple versions simultaneously.
3. **Canary Release**: This strategy involves deploying the new version to a small subset of users before rolling it out to the entire user base. This approach allows for real-world testing and minimizes risk by limiting exposure initially.
6. **Immutable Infrastructure**: Rebuild and replace infrastructure with each deployment rather than updating existing systems. This ensures consistency and mitigates configuration drift, though it may require more sophisticated infrastructure management.

## Decision Outcome

Chosen option: Canary Release, because this approach allows us to gradually roll out changes to a small subset of users, monitoring the impact before wider deployment. By leveraging canary releases, we can identify potential issues early, minimizing risks and ensuring a more stable user experience. 

### Consequences

* Good, this strategy allows us to monitor and address any issues promptly, ensuring a stable and reliable experience for the majority of our user base. This careful approach enhances user trust and satisfaction, supporting AML's objectives of growth and retention. With a more reliable deployment process, user engagement is likely to improve, aiding in the achievement of our target of a 10% annual user base increase. The strategy effectively aligns with our goals by fostering a dependable and positive user experience.

### Confirmation

The success of a canary release deployment strategy can be confirmed by monitoring key performance indicators and user feedback to ensure the new version performs as expected without negatively impacting the user experience.

## More Information

This approach is particularly beneficial over rolling deployment and immutable infrastructure when dealing with legacy systems that are vastly different from the new system. The incremental exposure allows for close monitoring and validation of the new system's performance and compatibility without impacting the entire user base. This reduces the risk of widespread failure and provides an opportunity to gather feedback and make data-driven decisions before a full-scale deployment.

### References

Xia, T., Bhardwaj, S., Dmitriev, P., & Fabijan, A. (2019, May). Safe velocity: a practical guide to software deployment at scale using controlled rollout. In 2019 IEEE/ACM 41st International Conference on Software Engineering: Software Engineering in Practice (ICSE-SEIP) (pp. 11-20). IEEE.
Tarvo, A., Sweeney, P. F., Mitchell, N., Rajan, V. T., Arnold, M., & Baldini, I. (2015, July). CanaryAdvisor: a statistical-based tool for canary testing. In Proceedings of the 2015 International Symposium on Software Testing and Analysis (pp. 418-422).
Dearle, A. (2007, May). Software deployment, past, present and future. In Future of Software Engineering (FOSE'07) (pp. 269-284). IEEE.
