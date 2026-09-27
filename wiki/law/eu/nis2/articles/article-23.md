---
type: Law
title: 'Article 23: Reporting Obligations'
description: Establishes the mandatory multi-stage incident reporting framework with
  strict 24h, 72h, and 1-month statutory clocks.
category: law
tags:
- nis2
- directive
- article
- article-23
status: draft
generated:
  by: agent:antigravity
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
  provision: Article 23
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

**Article 23 (Reporting obligations)** establishes the Union-wide incident notification framework for essential and important entities experiencing a **significant incident**[^directive-eu-2022-2555].

Article 23 replaces the vague notification timelines of NIS1 with an unambiguous, multi-stage notification clock enforced across all 27 EU Member States.

# The Multi-Stage Incident Reporting Clock

```
   INCIDENT DETECTED
           |
           | T + 24 Hours
           v
+-------------------------------------------------------------+
| 1. Early Warning (Article 23(4)(a))                         |
| - Notify CSIRT or competent authority                       |
| - State whether incident is suspected of being caused by    |
|   unlawful or malicious acts                                |
| - State whether it could have cross-border impact           |
+-------------------------------------------------------------+
           |
           | T + 72 Hours
           v
+-------------------------------------------------------------+
| 2. Incident Notification (Article 23(4)(b))                 |
| - Update early warning information                          |
| - Provide initial assessment: severity, impact, indicators   |
+-------------------------------------------------------------+
           |
           | T + 1 Month (or Intermediate Report on request)
           v
+-------------------------------------------------------------+
| 3. Final Report (Article 23(4)(e))                          |
| - Detailed description of incident, severity, and impact    |
| - Type of threat or root cause                              |
| - Applied and ongoing mitigation measures                   |
| - Cross-border impact details                               |
+-------------------------------------------------------------+
```

# Significant Incident Thresholds (Article 23(3))
An incident is considered significant if:
1. It has caused or is capable of causing severe operational disruption of the services or financial loss for the entity concerned;
2. It has affected or is capable of affecting other natural or legal persons by causing considerable material or non-material damage.

# Related concepts
- [Article 20: Governance](article-20.md)
- [Article 21: Cybersecurity Risk-Management Measures](article-21.md)
- [Incident Reporting Clocks Overview](../../../../obligations/reporting/incident-reporting-clocks.md)
[^directive-eu-2022-2555]: European Parliament and Council of the European Union, Directive (EU) 2022/2555 on measures for a high common level of cybersecurity across the Union (NIS2), http://data.europa.eu/eli/dir/2022/2555/oj
