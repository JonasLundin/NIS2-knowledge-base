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
    across the Union (NIS 2 Directive)
  author: European Parliament and Council of the European Union
  last_modified: '2022-12-27T00:00:00Z'
x-nis2:
  jurisdiction: EU
  authority_level: binding
  instrument_status: in_force
  provision: Article 23
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

Article 23 establishes the multi-stage incident reporting process for essential and important entities experiencing a **significant incident**[^directive-eu-2022-2555].

# Mandatory Reporting Windows

1. **Early Warning (within 24 hours)** of becoming aware of the significant incident:
   - Must indicate whether the significant incident is suspected of being caused by unlawful or malicious acts or could have an cross-border impact.
   - *Trust Service Providers*: Under Article 23(4) final subparagraph, trust service providers must notify competent authorities or CSIRTs within 24 hours of becoming aware of any incident having a significant impact.
2. **Incident Notification (within 72 hours)** of becoming aware:
   - Initial assessment of the incident, updating the early warning and indicating severity, impact, and indicators of compromise where available.
3. **Intermediate Report (upon request)**:
   - Status update requested by the CSIRT or competent authority.
4. **Final Report (within 1 month after the 72-hour notification)** under point (b):
   - Detailed description of the incident, including its severity and impact.
   - Type of threat or root cause that likely triggered the incident.
   - Applied and ongoing mitigation measures.
   - Cross-border impact where relevant.
5. **Progress Report (if incident is ongoing)**:
   - If the incident is still ongoing at the 1-month mark, a progress report must be submitted at that time, followed by a final report within one month after handling the incident.

# Related concepts
- [Incident Reporting Obligations](../../../../obligations/reporting/incident-reporting-clocks.md)
- [Implementing Regulation (EU) 2024/2690](../secondary-legislation/implementing-regulation-2024-2690.md)

[^directive-eu-2022-2555]: European Parliament and Council of the European Union, Directive (EU) 2022/2555 on measures for a high common level of cybersecurity across the Union (NIS 2 Directive), http://data.europa.eu/eli/dir/2022/2555/oj
