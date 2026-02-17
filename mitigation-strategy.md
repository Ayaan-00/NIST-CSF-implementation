# Security Mitigation Strategy

**Framework:** NIST CSF 2.0
**Scope:** Organisation-wide
**Approach:** Open-source tools prioritized for cost-effectiveness and scalability

---

## Objectives

- Mitigate high and medium-priority cybersecurity risks identified in the Risk Assessment
- Apply short- and mid-term open-source solutions that are cost-effective and scalable
- Align mitigation efforts with NIST CSF 2.0 functions and subcategories
- Ensure controls are practical and manageable for a small business with limited technical resources

---

## Risk Treatment Matrix

| Risk ID | Description | Asset Type | Impact | Priority | Mitigation Summary | Timeline |
|---------|-------------|-----------|--------|----------|-------------------|----------|
| R-01 | Phishing leading to credential theft | People / Email | 5 | High (P1) | MFA, password manager, awareness training | 0 to 60 Days |
| R-02 | Endpoint malware | Endpoints / Software | 4 | Medium (P2) | ClamAV, patch management, least privilege | 60 to 180 Days |
| R-03 | Data loss via ransomware | Informational / Storage | 5 | High (P1) | Encrypted backups, spam filter, training | 0 to 60 Days |
| R-04 | Unauthorized remote access | Services / VPN | 4 | Medium (P2) | VPN configuration, RBAC, MFA | 120 to 180 Days |
| R-05 | Insider misuse of data | People / Files | 3 | Medium (P3) | RBAC, logging, awareness training | 120 to 180 Days |
| R-06 | Weak patch management | Software / OS | 4 | Medium (P3) | Automated patching, vulnerability scanning | 60 to 120 Days |
| R-07 | Lack of security monitoring | Systems / Logs | 4 | Medium (P2) | SIEM deployment, alerting, dashboard reviews | 120 to 180 Days |
| R-08 | Poor password hygiene | People / Systems | 5 | High (P1) | Password manager, MFA, quarterly reviews | 0 to 60 Days |

---

## Detailed Mitigation Plans

### R-01: Phishing Leading to Credential Theft

- **Control Objectives:** Prevent unauthorized access to business accounts
- **Measures:** Deploy Bitwarden for secure password storage. Implement MFA using Bitwarden or Keycloak. Conduct quarterly phishing simulations via GoPhish. Deliver awareness training through LMS.
- **Mapped Tools:** Bitwarden, GoPhish, MFA
- **Responsible Role:** IT Admin / Training Coordinator
- **NIST CSF Functions:** PR.AC, DE.CM, RS.AN

### R-02: Endpoint Malware

- **Control Objectives:** Prevent malware infection on business devices
- **Measures:** Deploy ClamAV on all endpoints. Enforce RBAC to limit privileges. Automate patching using Lynis. Configure Wazuh alerts for threat detection.
- **Mapped Tools:** ClamAV, Lynis, Wazuh
- **Responsible Role:** IT Admin
- **NIST CSF Functions:** PR.IP, DE.CM, RC.RP

### R-03: Data Loss via Ransomware

- **Control Objectives:** Ensure availability and recoverability of business data
- **Measures:** Implement daily encrypted backups via Duplicati. Maintain long-term backups using Restic. Use SpamAssassin to filter email attachments. Train employees on safe file handling. Test backup recovery monthly.
- **Mapped Tools:** Duplicati, Restic, SpamAssassin
- **Responsible Role:** IT + Ops Lead
- **NIST CSF Functions:** PR.DS, RC.IM, RS.RP

### R-04: Unauthorized Remote Access

- **Control Objectives:** Secure remote access to systems and data
- **Measures:** Configure WireGuard or OpenVPN for secure tunneling. Enforce MFA for VPN access. Apply RBAC through Keycloak. Monitor access logs via Wazuh.
- **Mapped Tools:** OpenVPN, WireGuard, MFA, Keycloak
- **Responsible Role:** Network Admin
- **NIST CSF Functions:** ID.AM, PR.AC, DE.CM

### R-05: Insider Misuse of Data

- **Control Objectives:** Prevent unauthorized internal data access
- **Measures:** Enforce RBAC using Keycloak. Enable and review Wazuh logs weekly. Include insider threat topics in security awareness training. Strengthen onboarding and offboarding access controls.
- **Mapped Tools:** Wazuh, Keycloak
- **Responsible Role:** HR + Security Officer
- **NIST CSF Functions:** DE.DP, RS.AN, RC.CO

### R-06: Weak Patch Management

- **Control Objectives:** Keep systems up to date and vulnerability-free
- **Measures:** Automate OS patching via native tools. Use Lynis to scan for outdated packages. Maintain a patch tracking spreadsheet.
- **Mapped Tools:** Lynis, OS-native updaters
- **Responsible Role:** IT Support
- **NIST CSF Functions:** PR.IP, ID.AM

### R-07: Lack of Security Monitoring

- **Control Objectives:** Detect threats and anomalous behavior promptly
- **Measures:** Deploy Wazuh SIEM to aggregate and monitor logs. Configure detection rules and alerts. Regularly review dashboard metrics.
- **Mapped Tools:** Wazuh
- **Responsible Role:** Security Admin
- **NIST CSF Functions:** DE.CM, DE.DP

### R-08: Poor Password Hygiene

- **Control Objectives:** Enforce strong authentication practices
- **Measures:** Adopt Bitwarden for password storage and generation. Train staff on password best practices. Require use of password generator. Conduct quarterly password health reviews.
- **Mapped Tools:** Bitwarden
- **Responsible Role:** IT Admin / HR
- **NIST CSF Functions:** PR.AC, PR.AT

---

## Implementation Roadmap

| Phase | Focus Areas | Key Tools | Timeline |
|-------|------------|-----------|----------|
| Phase 1 (P1) | MFA, password management, backup, phishing training | Bitwarden, Duplicati, GoPhish | 0 to 60 Days |
| Phase 2 (P2) | Endpoint AV, SIEM, VPN, patch management | ClamAV, Wazuh, OpenVPN, Lynis | 60 to 180 Days |
| Phase 3 (P3) | ZTNA, insider monitoring, role-based access control | Keycloak, Cloudflare Access, Wazuh | 180 to 300 Days |
| Phase 4 (Ongoing) | Awareness refresh, log review, audit and compliance | SIEM dashboards, LMS, NIST benchmarks | Quarterly |

---

## Control-to-Risk Coverage

| Control / Tool | Risks Covered | Priority | Category |
|----------------|--------------|----------|----------|
| Bitwarden | R-01, R-08 | P1 | Short-Term |
| GoPhish | R-01 | P1 | Short-Term |
| MFA (Bitwarden/OpenVPN) | R-01, R-04, R-08 | P1 | Short-Term |
| Duplicati / Restic | R-03 | P1 | Short-Term |
| SpamAssassin | R-03 | P1 | Short-Term |
| ClamAV | R-02 | P2 | Short-Term |
| Lynis | R-02, R-06 | P2 | Short-Term |
| OpenVPN / WireGuard | R-04 | P2 | Mid-Term |
| Wazuh | R-05, R-07 | P2 | Mid-Term |
| Keycloak | R-04, R-05 | P2 | Mid-Term |

---

## NIST CSF 2.0 Control Mapping

| NIST Function | Subcategory | Applied Controls / Tools |
|--------------|-------------|------------------------|
| Identify (ID.AM) | Asset Inventory | Lynis, Patch Logs |
| Protect (PR.AC) | Access Control | Keycloak, MFA, RBAC |
| Protect (PR.IP) | Patch Management | Lynis, OS Auto Updates |
| Protect (PR.DS) | Data Security | Restic, Duplicati |
| Detect (DE.CM) | Continuous Monitoring | Wazuh, SIEM Rules |
| Respond (RS.AN) | Phishing Awareness | GoPhish, LMS Modules |
| Recover (RC.RP) | Recovery Plan | Backup Schedules, Testing |
