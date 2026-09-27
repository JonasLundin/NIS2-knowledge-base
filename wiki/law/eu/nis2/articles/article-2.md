---
type: Law
title: 'Article 2: Scope & Size-Cap Rule'
description: Defines personal and material scope of NIS2 based on the size-cap rule
  (medium and large enterprises) and specific exceptions.
category: law
tags:
- nis2
- directive
- article
- article-2
- scope
- size-cap
status: draft
generated:
  by: agent:kb-researcher-writer
  at: '2026-09-27T00:00:00Z'
stale_after: '2027-12-31T00:00:00Z'
sources:
- id: directive-eu-2022-2555
  resource: http://data.europa.eu/eli/dir/2022/2555/oj
  title: Directive (EU) 2022/2555 on measures for a high common level of cybersecurity
    across the Union (NIS2)
  author: European Parliament and Council of the European Union
  last_modified: '2022-12-14T00:00:00Z'
x-nis2:
  jurisdiction: EU
  authority_level: binding
  instrument_status: in_force
  provision: Article 2
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

**Article 2 (Scope)** establishes the personal and material application threshold of Directive (EU) 2022/2555 (NIS2)[^directive-eu-2022-2555].

Unlike NIS1, which left operator identification to fragmented national discretion, NIS2 introduces the uniform **"Size-Cap Rule"**: all entities that qualify as medium-sized enterprises or exceed the ceilings for medium-sized enterprises operating within Annex I or Annex II sectors are automatically in scope.

# The Size-Cap Thresholds (Commission Recommendation 2003/361/EC)

```
+-------------------------------------------------------------------+
|               NIS2 SIZE-CAP DETERMINATION MATRIX                  |
+-------------------------------------------------------------------+
| ENTERPRISE SIZE      | EMPLOYEES        | ANNUAL TURNOVER / BALANCE|
+----------------------+------------------+-------------------------+
| Small / Micro        | < 50 staff       | <= €10 million          |
| (Generally out of    |                  |                         |
| scope unless critical)                  |                         |
+----------------------+------------------+-------------------------+
| Medium-Sized         | 50 to 249 staff  | <= €50 million turnover |
| (IN SCOPE)           |                  | or <= €43m balance sheet|
+----------------------+------------------+-------------------------+
| Large                | >= 250 staff     | > €50 million turnover  |
| (IN SCOPE)           |                  | or > €43m balance sheet |
+-------------------------------------------------------------------+
```

# Exceptions: Small / Micro Entities Brought In Scope (Article 2(2))
Regardless of their size, micro and small entities are brought under NIS2 if:
1. Services are provided by providers of public electronic communications networks or publicly available electronic communications services;
2. Trust service providers;
3. Top-level domain name (TLD) name registries and DNS service providers;
4. Sole provider of a service in a Member State essential for critical societal or economic activities;
5. Potential disruption could induce significant systemic risk, cross-border impact, or critical societal disruptions;
6. Critical entities under Directive (EU) 2022/2557 (CER Directive).

# Related concepts
- [Articles Index](index.md)
- [Article 3: Essential and Important Entities](article-3.md)
- [Annex I: Sectors of High Criticality](../annexes/annex-1.md)
- [Annex II: Other Critical Sectors](../annexes/annex-2.md)

[^directive-eu-2022-2555]: European Parliament and Council of the European Union, Directive (EU) 2022/2555 on measures for a high common level of cybersecurity across the Union (NIS2), http://data.europa.eu/eli/dir/2022/2555/oj
