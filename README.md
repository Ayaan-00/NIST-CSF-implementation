# NIST CSF 2.0 Security Program Implementation: Small Business Case Study

A complete cybersecurity program built for a small business client with no existing security controls, aligned to the NIST Cybersecurity Framework 2.0.

---

## Project Overview

This repository documents a security consulting engagement where I designed and delivered a full cybersecurity program for a small construction company operating with no formal security controls, no dedicated IT security staff, and a non-technical workforce.

The project ran from January to March 2025 and produced actionable deliverables across all five NIST CSF 2.0 functions: **Identify, Protect, Detect, Respond, and Recover.** Every recommendation was built around open-source tools and realistic implementation timelines appropriate for a small business with limited budget and technical resources.

This was not a theoretical exercise. The client had real operational gaps: unpatched systems, no endpoint protection, no backup strategy, default passwords on network equipment, and employees with zero security awareness training. The deliverables in this repository addressed those gaps with practical, implementable solutions.

**All client-identifying information has been removed.** Company names, employee names, contact details, and location-specific data have been replaced with placeholders to protect client confidentiality.

---

## My Role

I served as a security consultant on a small team responsible for assessing the client's risk posture and building the security program from the ground up. My contributions included:

- Conducting the full risk assessment using the OCTAVE methodology across informational, physical, and service assets
- Mapping identified risks to NIST CSF 2.0 functions, NIST SP 800-53 Rev 5, ISO/IEC 27001:2022, and CIS Controls v8
- Developing the mitigation strategy with a phased implementation roadmap
- Authoring security policies tailored to the client's operational context
- Researching and recommending open-source tools for each control category
- Contributing to the Business Impact Analysis and Business Continuity Plan

---

## Deliverables

### Core Assessments and Strategy

| Deliverable | Description |
|-------------|-------------|
| **Risk Assessment** | Multi-sheet assessment using the OCTAVE approach. 18 identified risks scored across informational, physical, and service assets. Each risk mapped to NIST CSF 2.0, NIST 800-53, ISO 27001, and CIS Controls v8. Includes risk priority numbers, treatment decisions, residual risk tracking, and leadership approval. |
| **Business Impact Analysis** | Identifies critical business functions, downtime tolerances (MTD, RTO, RPO), dependencies, threat awareness, recovery prioritization, and compliance gaps. Includes a readiness self-assessment and framework alignment audit. |
| **Mitigation Strategy** | Risk treatment matrix covering 8 priority risks with specific control objectives, mapped open-source tools, responsible roles, implementation timelines, and NIST CSF function alignment. Includes a 4-phase roadmap from immediate actions through ongoing operations. |
| **Cyber Tool Kit** | Comprehensive guide to open-source security tools organized by control category: endpoint protection, firewalls, VPN, SIEM, IAM, patch management, phishing simulation, backup and recovery, email and web security. Includes installation and configuration guides for each tool. |
| **Cybersecurity Roadmap** | Visual timeline of the implementation plan from immediate priorities through long-term objectives. |

### Security Policies

Each policy was written to be practical and enforceable for a small business without a dedicated security team. All policies include version control, review and approval logs, scope definitions, and compliance references.

| Policy | NIST CSF Alignment |
|--------|-------------------|
| Information Security Policy | GV.PO, GV.RR |
| Access Control Policy | PR.AA, PR.AC |
| Acceptable Use Policy | PR.AT, GV.PO |
| Incident Response Plan | RS.RP, RS.CO, RS.AN, RS.MI |
| Data Breach Response Policy | RS.CO, RS.RP |
| Business Continuity Plan | RC.RP, RC.CO |
| Network Security Policy | PR.DS, PR.PT, DE.CM |
| Endpoint Security Policy | PR.DS, DE.CM |
| Cloud Security Policy | PR.DS, PR.AA |
| Patch Management Policy | PR.IP, ID.AM |
| Log Management and Monitoring Policy | DE.CM, DE.AE |
| Mobile Device Management Policy | PR.DS, PR.AC |
| Third-Party and Vendor Security Policy | GV.SC, ID.RA |

---

## Framework Alignment

The entire program maps to multiple industry frameworks, with NIST CSF 2.0 as the primary structure.

| Framework | How It Was Applied |
|-----------|-------------------|
| **NIST CSF 2.0** | Primary organizing framework. All deliverables mapped to CSF functions and subcategories. |
| **NIST SP 800-53 Rev 5** | Specific controls referenced for each CSF subcategory in the controls mapping document. |
| **ISO/IEC 27001:2022** | Cross-referenced in the risk assessment for organizations pursuing formal certification. |
| **CIS Controls v8** | Mapped alongside NIST controls to provide an alternative implementation benchmark. |
| **OCTAVE** | Risk assessment methodology used for asset classification and threat-vulnerability pairing. |

---

## Implementation Roadmap

The mitigation strategy follows a phased approach designed for a small business with limited resources.

**Phase 1 (0 to 60 Days):** MFA deployment, password manager rollout (Bitwarden), automated backups (Duplicati), phishing awareness training (GoPhish)

**Phase 2 (60 to 180 Days):** Endpoint antivirus (ClamAV), SIEM deployment (Wazuh), VPN configuration (OpenVPN/WireGuard), patch management automation (Lynis)

**Phase 3 (180 to 300 Days):** Zero Trust network access (Keycloak, Cloudflare Access), insider threat monitoring, role-based access control enforcement

**Phase 4 (Ongoing):** Quarterly awareness refreshers, SIEM dashboard reviews, log audits, compliance benchmarking against NIST CSF

---

## Tools Recommended

All tools selected are open-source or free-tier, prioritizing cost-effectiveness for a small business.

| Category | Tools |
|----------|-------|
| Password Management | Bitwarden |
| Endpoint Protection | ClamAV |
| SIEM and Logging | Wazuh |
| Vulnerability Scanning | Lynis |
| VPN and Remote Access | OpenVPN, WireGuard |
| Identity and Access Management | Keycloak |
| Phishing Simulation | GoPhish |
| Backup and Recovery | Duplicati, Restic |
| Email Filtering | SpamAssassin |
| Zero Trust Access | Cloudflare Access |

---

## Repository Structure

```
├── README.md
├── assessments/
│   ├── risk-assessment-summary.md
│   └── business-impact-analysis-summary.md
├── strategy/
│   ├── mitigation-strategy.md
│   └── cybersecurity-roadmap.png
├── policies/
│   ├── information-security-policy.md
│   ├── access-control-policy.md
│   ├── acceptable-use-policy.md
│   ├── incident-response-plan.md
│   ├── data-breach-response-policy.md
│   ├── business-continuity-plan.md
│   ├── network-security-policy.md
│   ├── endpoint-security-policy.md
│   ├── cloud-security-policy.md
│   ├── patch-management-policy.md
│   ├── log-management-monitoring-policy.md
│   ├── mobile-device-management-policy.md
│   └── third-party-vendor-security-policy.md
└── framework/
    ├── nist-csf-controls-mapping.md
    └── nist-csf-functions-and-categories.md
```

---

## About Me

Cybersecurity professional based in Toronto. MS in Information Systems Security Management from Northeastern University. My experience includes SOC operations, penetration testing, web application security assessments, and security program development aligned to NIST CSF and SP 800-53 frameworks.

[LinkedIn](https://www.linkedin.com/in/ayaan-m-2643122a0/)

---

*This repository documents authorized consulting work. All client-identifying information has been removed to protect organizational privacy. Company names, employee names, and location-specific details have been replaced with generic placeholders.*
