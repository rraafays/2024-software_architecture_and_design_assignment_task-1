---
parent: Decisions
nav_order: 100
title: Choice of Frontend

# status: accepted
# date: 2024-10-01
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Frontend Web Technology

## Context and Problem Statement

Currently, the customer facing frontend for AML appears to be a monolithic inclusion with their legacy system and it is not well suited for a completely digital solution.

## Considered Options

* Next.js
* React
* HTML, CSS, JS

## Decision Outcome

Chosen option: Next.js, because it is the most supported and most feature filled frontend framework which allows the use of Typescript which will ensure high levels of maintainability due to code clarity. Many features included with Next.js are features that other frontends require plugins to gain which makes Next.js much better OOTB.

### Consequences

* Good, because it is extremely well supported and currently the most widely used framework it will allow for very easy and efficeint development and due to its popularity there are many plugins to allow for more complex frontends stylistically and functionality wise.

### Confirmation

This ADR will be confirmed by the success of the system's customer facing website UI amongst Library Members and Guests.

## More Information

Since we are experienced with Typescript and because Next.js is popular it makes for much more efficient development.

### References

Lazuardy, M. F. S., & Anggraini, D. (2022). Modern front end web architectures with react. js and next. js. Research Journal of Advanced Engineering and Science, 7(1), 132-141.
Aggarwal, S. (2018). Modern web-development using reactjs. International Journal of Recent Research Aspects, 5(1), 133-137.
O’rinboev, A. (2023). ANALYZING THE EFFICIENCY AND PERFORMANCE OPTIMIZATION TECHNIQUES OF REACT. JS IN MODERN WEB DEVELOPMENT. Инновационные исследования в современном мире: теория и практика, 2(24), 54-57.
