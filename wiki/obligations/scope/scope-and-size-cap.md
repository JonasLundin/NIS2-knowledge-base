---
type: Requirement
title: NIS2 Scope and the Size-Cap Rule (Articles 2 & 3)
description: Detailed criteria determining essential versus important entities based
  on headcount, turnover, and criticality.
category: requirement
tags:
- nis2
- obligations
- scope
- article-2
- size-cap
- essential-entity
status: draft
generated:
  by: agent:kb-researcher-writer
  at: '2026-09-27T00:00:00Z'
stale_after: '2027-12-31T00:00:00Z'
sources:
- id: recommendation-2003-361-ec
  resource: http://data.europa.eu/eli/reco/2003/361/oj
  title: Commission Recommendation 2003/361/EC concerning the definition of micro,
    small and medium-sized enterprises
  author: European Commission
  last_modified: '2003-05-20T00:00:00Z'
- id: directive-eu-2022-2555
  resource: http://data.europa.eu/eli/dir/2022/2555/oj
  title: Directive (EU) 2022/2555 on measures for a high common level of cybersecurity
    across the Union (NIS 2 Directive)
  author: European Parliament and Council of the European Union
  last_modified: '2022-12-27T00:00:00Z'
x-nis2:
  jurisdiction: EU
  authority_level: binding
  instrument_status: in_force
  provision: Articles 2, 3
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

Directive (EU) 2022/2555 relies on the enterprise size definitions in Commission Recommendation 2003/361/EC to establish regulatory applicability and distinguish essential from important entities[^recommendation-2003-361-ec][^directive-eu-2022-2555].

# SME Thresholds (Recommendation 2003/361/EC)

- **Small Enterprise (Excluded Baseline)**:
  - Fewer than 50 staff headcount; AND
  - Annual turnover not exceeding EUR 10 million or balance sheet total not exceeding EUR 10 million.
  - Small and micro enterprises are excluded from default NIS2 scope, unless designated under Article 2(2) (e.g. DNS, TLDs, sole providers, or CER critical entities).
- **Medium-Sized Enterprise**:
  - Staff headcount between 50 and 249; AND
  - Annual turnover not exceeding EUR 50 million or balance sheet total not exceeding EUR 43 million (and exceeding the small enterprise ceiling).
- **Large Enterprise**:
  - 250 or more staff headcount; OR
  - Annual turnover exceeding EUR 50 million and balance sheet total exceeding EUR 43 million.

# Regulatory Consequence of Size Thresholds
- **Annex I Sectors**: Large enterprises are classified as **essential entities** (Article 3(1)(a)). Medium-sized enterprises are classified as **important entities** (Article 3(2)).
- **Annex II Sectors**: Both medium-sized and large enterprises are classified as **important entities** (Article 3(2)).

# Related concepts
- [Article 2 Scope](../../law/eu/nis2/articles/article-2.md)
- [Article 3 Classification](../../law/eu/nis2/articles/article-3.md)

[^recommendation-2003-361-ec]: European Commission, Commission Recommendation 2003/361/EC concerning the definition of micro, small and medium-sized enterprises, http://data.europa.eu/eli/reco/2003/361/oj
[^directive-eu-2022-2555]: European Parliament and Council of the European Union, Directive (EU) 2022/2555 on measures for a high common level of cybersecurity across the Union (NIS 2 Directive), http://data.europa.eu/eli/dir/2022/2555/oj
