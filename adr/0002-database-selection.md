---
parent: Decisions
nav_order: 100
title: Decide on Database Technology

# status: accepted
# date: 2024-10-01
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Database

## Context and Problem Statement

We need to decide upon a technology to store our systems' information which may range from private sensitive information such as user information to public information such as the media items AML offer to Library Members.

## Considered Options

* MySQL
* PostgreSQL
* SQLite

## Decision Outcome

Chosen option: SQLite, because it is a simple easy to maintain solution which still allows for high security and scaling. Additionally, it allows for fragmentation of the database into shards into the future which increase both security and also performance. 

### Consequences

* Good, because it allows for the security which AML needs as well as accounts for any possible future expansion and does all of this while still being relatively easy to port to a new server in an emergency or for backup purposes.

### Confirmation

This ADR will be confirmed by the success of the database when it comes to security and backup.

## More Information

SQLite offers a very low barrier to entry for inexperienced developers and maintainers since it is inherently designed to be very simple and easy to understand and only offer the absolute necessary. Leaving a lot of freedom to developers and entrusting them with things such as encryption. 

### References

Bhosale, S. T., Patil, T., & Patil, P. (2015). Sqlite: Light database system. Int. J. Comput. Sci. Mob. Comput, 44(4), 882-885.
Douglas, K., & Douglas, S. (2003). PostgreSQL: a comprehensive guide to building, programming, and administering PostgresSQL databases. SAMS publishing.
DuBois, P. (2013). MySQL. Addison-Wesley.
