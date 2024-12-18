---
parent: Decisions
nav_order: 100
title: Methods of Security

# status: accepted
# date: 04-11-2024
# decision-makers: Raf, Veronica,
# consulted: Essam, Bassu, Rizwana
# informed: Essame, Veronica, Raf
---
<!-- markdownlint-disable-next-line MD025 -->
# Data Security

## Context and Problem Statement

It has not been disclosed what kind of security AML currently has inplace in their legacy system however, it is therefore absolutely necessary and inherent to the creation of a new system to update whatever security methods were used by AML previously.

## Considered Options

* Strapi built in encryption
* SQLite encryption
* Server encryption

## Decision Outcome

Chosen option: Strapi built in encryption. Both encrypting SQLite and the Server's internal data itself are completely viable however, since all data is processed via our CMS (Strapi) in this new system it makes more sense efficiency wise to have Strapi handle this encryption which by default is highly secure due to data encryption being core to its design.

### Consequences

* Good, because not only does it achieve both of the other considered options indirectly. It also has a huge following meaning that encryption will always be developed due to it being free open source software which means that vulnerabilities if they are ever found will be patched without AML requiring that specific area of the system to be maintained.

### Confirmation

This ADR will be confirmed by the compliance of the system to British GDPR rules.

## More Information

Strapi has an excellent track record due to its open source nature with patching vulnerabilities and it is also designed in such a way that further layers of encryption may be added in the future if deemed necessary.

### References

STRAPI, the leading open-source headless CMS. Strapi, the leading open-source headless CMS. (n.d.). https://strapi.io/security
