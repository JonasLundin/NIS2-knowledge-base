---
type: Requirement
title: Cybersecurity Risk-Management Measures
description: Comprehensive analysis of the ten statutory risk management requirements
  under NIS2 Article 21.
category: requirement
tags:
- nis2
- obligation
- risk-management-measures
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
  provision: Article 21
  checked_at: '2026-09-27T00:00:00Z'
---

# Summary

The **Cybersecurity Risk-Management Measures** established under Article 21 of Directive (EU) 2022/2555 (NIS2) form the mandatory baseline for information security across European critical infrastructure and digital service providers[^directive-eu-2022-2555].

# Operational Implementation Blueprint

1. **Risk Analysis and Security Policies**: Formal risk assessment methodology aligned with ISO/IEC 27001 or NIST CSF 2.0.
2. **Incident Handling**: 24/7 detection capabilities, Security Operations Center (SOC) playbooks, and SIEM/SOAR automation.
3. **Business Continuity**: Immutable off-site backups, disaster recovery sites, and periodic crisis simulation exercises.
4. **Supply Chain Security**: Vendor security vetting, contractual clauses, SBOM ingestion, and vulnerability monitoring.
5. **Vulnerability Handling**: Coordinated vulnerability disclosure (CVD) process, patch management SLAs, and penetration testing.
6. **Effectiveness Assessment**: Independent third-party cybersecurity audits and red-teaming exercises.
7. **Cyber Hygiene & Training**: Phishing simulations, role-based security training, and credential management.
8. **Cryptography**: Strict adherence to post-quantum readiness guidelines and robust TLS/AES standards.
9. **Access Control & HR Security**: Zero Trust architecture, principle of least privilege, and background checks.
10. **Multi-Factor Authentication (MFA)**: Phishing-resistant MFA (FIDO2/WebAuthn) for all remote access and administrative interfaces.

# Related concepts
- [Article 21: Cybersecurity Risk-Management Measures](../law/eu/nis2/articles/article-21.md)
- [Governance](governance.md)
- [Supply Chain Security](supply-chain-security.md)
[^directive-eu-2022-2555]: European Parliament and Council of the European Union, Directive (EU) 2022/2555 on measures for a high common level of cybersecurity across the Union (NIS2), http://data.europa.eu/eli/dir/2022/2555/oj
