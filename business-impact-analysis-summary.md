# Business Impact Analysis Summary

**Scope:** Organisation-wide: all departments
**Framework Alignment:** NIST CSF 2.0 (ID.AM, ID.RA, PR.IP)
**Status:** Completed and approved

---

## Purpose

This Business Impact Analysis identifies and evaluates the potential impact of disruptive cyber and physical events on the core operations of the organization. It establishes a foundation for prioritizing recovery strategies, continuity planning, and cybersecurity controls: particularly important for a small business with limited resources.

---

## Critical Business Functions

| Function | Department | Frequency | Dependencies |
|----------|-----------|-----------|-------------|
| Project Management | Operations | Daily | Spreadsheets, email, paper schedules |
| Payroll and Accounting | Finance | Bi-weekly | Accounting software (local), USB drives, paper timesheets |
| Vendor Communications | Procurement | Daily | Email, phone, unprotected channels |
| Blueprint Storage | Engineering | Weekly | Shared folders on local PC or USB, printed copies |
| Site Surveillance | Security | 24/7 | DVR system, no remote access, local storage only |
| Employee Records | HR | Monthly | HR software, encrypted databases |

---

## Impact Assessment

| Impact Area | Severity | Notes |
|------------|----------|-------|
| Financial Loss | Severe | Delayed payroll or project stoppage can halt operations |
| Legal and Compliance | Moderate | Improper storage of employee and blueprint data may violate regulations |
| Customer Impact | Moderate | Delays in communication or project progress affect clients |
| Operational Delay | Severe | Data or system loss can halt construction, vendor work, and payroll |

---

## Downtime Tolerances

| Function | Max Tolerable Downtime | Recovery Time Objective | Recovery Point Objective |
|----------|----------------------|------------------------|------------------------|
| Payroll | 1 day | 8 hours | 4 hours |
| Project Management | 2 days | 24 hours | 6 hours |
| Vendor Communication | 2 days | 12 hours | 8 hours |
| Surveillance System | 1 day | 6 hours | 0 hours |

---

## Key Findings

The readiness self-assessment revealed significant gaps. The organization had no documented recovery procedures, no defined incident reporting process, no backup verification, no remote access capability, and no prior continuity training. Most business functions depended on local storage with no redundancy.

**Compliance alignment audit results:**

| Framework | Aligned | Gap |
|-----------|---------|-----|
| NIST CSF ID.AM (Asset Management) | No | No documented system inventory or owner assignment |
| NIST CSF ID.RA (Risk Assessment) | No | Risks identified informally, not tracked or reviewed |
| NIST CSF PR.IP (Information Protection) | No | No defined data protection or recovery policies |
| ISO/IEC 27001 Clauses 6 to 8 | No | No controls around planning, operations, or performance |
| CIS Controls | No | Controls not adopted or benchmarked |

These findings directly informed the mitigation strategy and policy development phases of the project.
