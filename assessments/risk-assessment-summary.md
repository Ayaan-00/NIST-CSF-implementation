# Risk Assessment Summary

**Methodology:** OCTAVE (Operationally Critical Threat, Asset, and Vulnerability Evaluation)
**Scope:** Organisation-wide: all departments
**Classification:** Internal
**Framework Mapping:** NIST CSF 2.0, NIST SP 800-53 Rev 5, ISO/IEC 27001:2022, CIS Controls v8

---

## Asset Inventory

The assessment began with a full asset inventory classifying organizational assets into three categories: informational, physical, and service. Each asset was scored for confidentiality, integrity, and availability to produce a composite asset value.

**25 assets identified** across:

- **Physical assets:** Desktops, laptops, routers, switches, smartphones, IoT security cameras, external storage, digital projectors
- **Informational assets:** HR management system, payroll software, cloud storage, ERP system
- **Service assets:** Email accounts, construction management software, antivirus, collaboration tools

Each asset was assigned an owner, custodian, classification level, and status.

---

## Risk Register

18 risks were identified, scored, and prioritized using impact and probability ratings (1 to 5 scale). Priority level is calculated as Impact × Probability.

| Risk ID | Description | Impact | Probability | Priority | Treatment |
|---------|-------------|--------|-------------|----------|-----------|
| R001 | Malware infection: lack of endpoint protection | 4 | 5 | 20 | Mitigate |
| R002 | Data loss due to hardware failure | 5 | 3 | 15 | Mitigate |
| R003 | Unauthorized access: weak passwords | 4 | 4 | 16 | Mitigate |
| R004 | Phishing attacks on users | 5 | 4 | 20 | Mitigate |
| R005 | Outdated OS vulnerabilities | 5 | 5 | 25 | Mitigate |
| R006 | Insider threat to HR data | 4 | 3 | 12 | Mitigate |
| R007 | Loss or theft of laptop | 3 | 3 | 9 | Mitigate |
| R008 | Unauthorized access to router | 5 | 2 | 10 | Mitigate |
| R009 | Misconfigured network switch | 4 | 4 | 16 | Mitigate |
| R010 | Phishing attacks on email accounts | 5 | 4 | 20 | Mitigate |
| R011 | Unauthorized access to IoT security cameras | 5 | 3 | 15 | Mitigate |
| R012 | Downtime of construction software | 5 | 2 | 10 | Mitigate |
| R013 | Data theft from external storage | 4 | 3 | 12 | Mitigate |
| R014 | Insider misuse of collaboration tool | 3 | 3 | 9 | Mitigate |
| R015 | Firmware vulnerabilities in networked devices | 4 | 3 | 12 | Mitigate |
| R016 | Data breach via insecure public Wi-Fi | 5 | 4 | 20 | Mitigate |
| R017 | Physical damage to laptops at job sites | 2 | 3 | 6 | Accept |
| R018 | Rogue devices connecting to router | 4 | 5 | 20 | Mitigate |

**Critical risks (Priority 20+):** Malware infection, phishing attacks, outdated OS vulnerabilities, insecure public Wi-Fi usage, and rogue network devices.

---

## Risk Treatment Approach

Each risk was evaluated against four treatment options: mitigate, avoid, transfer, or accept. For each mitigated risk, the assessment documents:

- Existing controls (what was already in place)
- Recommended mitigation or control strategy
- Responsible owner
- Expected and actual implementation dates
- Post-treatment residual risk values
- Leadership approval status

---

## Framework Cross-Mapping

Every risk in the assessment is mapped to:

| Framework | Example Mapping |
|-----------|----------------|
| NIST CSF 2.0 | PR.AC, DE.CM, RS.AN, ID.AM |
| NIST SP 800-53 Rev 5 | AC-2, SI-3, IR-4, CM-8 |
| ISO/IEC 27001:2022 | A.8.1, A.12.6, A.16.1 |
| CIS Controls v8 | CIS 1, CIS 4, CIS 10, CIS 17 |

This multi-framework mapping allows the organization to benchmark against different compliance requirements and supports future certification efforts.
