---
type: Requirement
title: Incident Reporting Clocks
description: Operational guidance on complying with the mandatory 24-hour, 72-hour,
  and 1-month reporting obligations under NIS2 Article 23.
category: requirement
tags:
- nis2
- obligation
- incident-reporting-clocks
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

The **Incident Reporting Clocks** under Directive (EU) 2022/2555 (NIS2) Article 23 impose legally binding notification deadlines on essential and important entities experiencing significant cybersecurity incidents[^directive-eu-2022-2555].

# Stage-by-Stage Operational Requirements

### 1. Early Warning (Within 24 Hours)
- **Deadline**: Within 24 hours of becoming aware of the significant incident.
- **Recipient**: National CSIRT or designated competent authority.
- **Content**: Initial alert indicating whether the incident is suspected of being caused by malicious activity and potential cross-border ramifications.

### 2. Incident Notification (Within 72 Hours)
- **Deadline**: Within 72 hours of becoming aware of the significant incident.
- **Content**: Comprehensive update on initial technical assessment, known indicators of compromise (IoCs), exploit vectors, and mitigation actions taken.

### 3. Intermediate Report
- **Trigger**: Upon request by the CSIRT or competent authority during an active investigation.

### 4. Final Report (Within 1 Month)
- **Deadline**: No later than 1 month after submission of the incident notification.
- **Content**: Exhaustive post-incident review, forensic root-cause analysis, total economic/operational impact, and permanent remediation measures implemented.

# Related concepts
- [Article 23: Reporting Obligations](../law/eu/nis2/articles/article-23.md)
- [Risk Management Measures](risk-management-measures.md)
[^directive-eu-2022-2555]: European Parliament and Council of the European Union, Directive (EU) 2022/2555 on measures for a high common level of cybersecurity across the Union (NIS2), http://data.europa.eu/eli/dir/2022/2555/oj
