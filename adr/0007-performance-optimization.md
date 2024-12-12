---
parent: Decisions
nav_order: 100
title: Performance Optimisation

# status: accepted
# date: 2024-10-01
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Performance Optimisation

## Context and Problem Statement

The AML's legacy system is reportedly unpopular among users and staff, a sentiment potentially attributed to its lack of performance optimisation.

## Considered Options

* Next.js Static Site Generation
* Strapi’s Caching 
* Content Delivery Network

## Decision Outcome

Chosen options: Next.js & Strapi's Caching, because Next.js static site generation enables us to pre-render pages at build time, resulting in fast load times and improved performance for end users. Strapi's built-in caching mechanisms will be utilized to store frequently accessed data, reducing response times and improving backend efficiency.

### Consequences


* Good, by combining these Performance Optimisation methods, our system aims to deliver a seamless and efficient user experience, meeting the performance demands of our new system.

### Confirmation

The success of a Next.js Static Site Generation & Strapi's Caching will be confirmed by regularly reviewing the metrics such as Page Load Time, Time to First Byte (TTFB), Core Web Vitals, Caching Efficiency, Load Testing, Resource Optimisation, and Database Performance using analytics and performance monitoring tools, adjusting our strategies as necessary to maintain and improve performance standards.

## More Information

We are leveraging Next.js static site generation along with Strapi's caching capabilities to enhance performance. However, should we decide to expand globally in the future—a move that is not currently a priority since AML has chosen to remain a UK-only service—we will consider integrating a Content Delivery Network (CDN). A CDN would distribute our content across multiple geographically distributed servers, reducing latency and improving load times for users around the world. This would ensure that our service remains fast and efficient, providing a seamless user experience regardless of the user's location.

### References

Petersen, H. (2016). From static and dynamic websites to static site generators. university of TARTU, Institute of Computer Science.
Patel, V. (2023). Analyzing the Impact of Next. JS on Site Performance and SEO. International Journal of Computer Applications Technology and Research, 12, 24-27.
Vakali, A., & Pallis, G. (2003). Content delivery networks: Status and trends. IEEE Internet Computing, 7(6), 68-74.
