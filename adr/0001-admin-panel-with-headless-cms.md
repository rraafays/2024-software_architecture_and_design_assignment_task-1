---
parent: Decisions
nav_order: 100
title: Replace Legacy CMS

# status: accepted
# date: 2024-10-01
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Headless Content Management System

## Context and Problem Statement

Currently, AML uses a legacy CMS system which is evident in the case study. This legacy CMS system is a limiting factor for AML. Switching to a headless CMS provides AML with far more options as well as ensuring that they have access to an admin panel without needing to create one from scratch.

## Considered Options

* Strapi
* Sanity
* WordPress VIP

## Decision Outcome

Chosen option: Strapi, because it is the only one of the options that is completely free, open source and also its user interface for its admin panel seems to be the most well-thought-out and user-friendly for non-technical users. Additionally, it is able to use a wide range of plugins which will make development much easier than the other options considered.

### Consequences

* Good, because it is free it will have very little impact on AML's finances due to a lack of a subscription service associated with its usage. Additionally it has seen mass adoption and has become a trusted free CMS system.

### Confirmation

This ADR will be confirmed by the success of the system we are architecting for AML as this is a core service / component of this system which is fundamental to its operation.

## More Information

Since we are experienced with Strapi, it is both a safe and trustworthy bet for our solution system and most importantly it fits the criteria of the client AML perfectly.

### References

Nguyen, A. (2022). Building an E-commerce Website Using Next Js, Mantine, and Strapi.
Messenlehner, B., & Coleman, J. (2019). Building web apps with WordPress: WordPress as an application framework. O'Reilly Media.
