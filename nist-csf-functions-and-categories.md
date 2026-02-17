# NIST CSF 2.0: Functions and Categories Applied

This document summarizes which NIST CSF 2.0 functions and categories were implemented in this security program, and which were excluded based on the client's scope and operational needs.

---

## Functions Implemented

### Identify (ID)
Understand the organization's environment, assets, and risks.

| Category | Included | Rationale |
|----------|----------|-----------|
| ID.AM: Asset Management | Yes | Full asset inventory conducted across physical, informational, and service assets |
| ID.BE: Business Environment | Yes | Business functions and dependencies documented in BIA |
| ID.RA: Risk Assessment | Yes | 18 risks identified and scored using OCTAVE methodology |
| ID.GV: Governance | Yes | Security policies and program management documented |
| ID.RM: Risk Management Strategy | Excluded | Deferred: formal risk appetite statement not required at current maturity |
| ID.SC: Supply Chain Risk Management | Excluded | Deferred: limited third-party digital supply chain at this scale |

### Protect (PR)
Safeguard critical assets and ensure training.

| Category | Included | Rationale |
|----------|----------|-----------|
| PR.AC: Access Control | Yes | RBAC, MFA, password management implemented |
| PR.AT: Awareness and Training | Yes | Phishing simulation and security awareness training program |
| PR.DS: Data Security | Yes | Encryption, backup, and data protection controls |
| PR.IP: Information Protection | Yes | Patch management, baseline configurations |
| PR.MA: Maintenance | Yes | Controlled maintenance procedures documented |
| PR.PT: Protective Technology | Yes | Firewall, VPN, and boundary protection |

### Detect (DE)
Identify cybersecurity events in a timely manner.

| Category | Included | Rationale |
|----------|----------|-----------|
| DE.AE: Anomalies and Events | Yes | SIEM alerting and anomaly detection via Wazuh |
| DE.CM: Continuous Monitoring | Yes | Log aggregation and dashboard monitoring |
| DE.DP: Detection Processes | Yes | Detection rules and audit review processes |

### Respond (RS)
Take action to contain and mitigate incidents.

| Category | Included | Rationale |
|----------|----------|-----------|
| RS.RP: Response Planning | Yes | Incident Response Plan developed |
| RS.CO: Communications | Yes | Incident reporting and escalation procedures |
| RS.AN: Analysis | Yes | Incident handling and vulnerability analysis |
| RS.MI: Mitigation | Yes | Flaw remediation and incident containment |
| RS.IM: Improvements | Excluded | Deferred: requires operational incident data to implement |

### Recover (RC)
Restore operations and incorporate lessons learned.

| Category | Included | Rationale |
|----------|----------|-----------|
| RC.RP: Recovery Planning | Yes | Business Continuity Plan and contingency procedures |
| RC.IM: Improvements | Yes | Contingency plan testing and improvement cycle |
| RC.CO: Communications | Yes | Recovery status communication and training |

---

## Project Timeline Alignment

| Weeks | Focus | CSF Functions |
|-------|-------|---------------|
| 1 to 4 | Research and Risk Assessment | ID.AM, ID.BE, ID.RA, ID.GV |
| 5 to 8 | Tool Selection and Policy Development | PR.AC, PR.AT, PR.DS, PR.IP, PR.MA, PR.PT |
| 9 to 10 | Implementation and Training | DE.AE, DE.CM, DE.DP |
| 11 to 12 | Testing, Adjustments, and Presentation | RS.RP, RS.CO, RS.AN, RS.MI, RC.RP, RC.IM, RC.CO |
