# NIST Cybersecurity Framework (CSF) 2.0 Mapping

## Midwest HealthTech Solutions (MHTS)

**Organization:** Midwest HealthTech Solutions (MHTS)  
**Industry:** Healthcare Technology  
**Environment:** AWS + Microsoft 365, hybrid/remote workforce  
**Employees:** 250  
**Framework:** NIST Cybersecurity Framework (CSF) 2.0

## 1. Purpose

This document maps selected MHTS cybersecurity and governance controls to the six functions of NIST CSF 2.0: **Govern, Identify, Protect, Detect, Respond, and Recover**.

The objective is to demonstrate how an organization can translate risk assessment findings into a structured cybersecurity governance and risk-management program.

## 2. NIST CSF 2.0 Functions

| Function | Purpose |
|---|---|
| **Govern (GV)** | Establish and monitor cybersecurity risk-management strategy, expectations, and policies. |
| **Identify (ID)** | Understand organizational assets, risks, dependencies, and cybersecurity risk exposure. |
| **Protect (PR)** | Implement safeguards to manage cybersecurity risks. |
| **Detect (DE)** | Discover and analyze possible cybersecurity attacks and compromises. |
| **Respond (RS)** | Take action regarding a detected cybersecurity incident. |
| **Recover (RC)** | Restore affected assets and operations and communicate recovery activities. |

## 3. Control-to-CSF Mapping

| Control / Practice | NIST CSF 2.0 Function | Example Category | Current State | Gap / Recommendation |
|---|---|---|---|---|
| Risk Register | Govern / Identify | GV.RM / ID.RA | Implemented | Review risks quarterly and after major environmental changes. |
| Security Policies | Govern | GV.PO | Partially Implemented | Formalize annual policy review and approval process. |
| Asset Inventory | Identify | ID.AM | Partially Implemented | Maintain centralized inventory of endpoints, cloud resources, and critical applications. |
| Vulnerability Management | Identify / Protect | ID.RA / PR.PS | Partially Implemented | Establish recurring vulnerability scans and documented remediation SLAs. |
| MFA | Protect | PR.AA | Ineffective | Enforce MFA consistently and review enrollment. |
| Endpoint Protection / EDR | Protect / Detect | PR.PS / DE.CM | Partially Effective | Increase endpoint coverage and centralize alert monitoring. |
| Logging and SIEM | Detect | DE.CM | Partially Implemented | Improve centralized collection, retention, alerting, and correlation. |
| Incident Response Plan | Respond | RS.MA / RS.CO | Partially Implemented | Conduct tabletop exercises and define escalation responsibilities. |
| Business Continuity / Disaster Recovery | Recover | RC.RP | Partially Implemented | Test restoration procedures and document recovery priorities. |
| Third-Party Risk Management | Govern / Identify | GV.SC / ID.RA | Partially Implemented | Establish formal vendor risk assessments and security requirements. |
| Least Privilege / RBAC | Protect | PR.AA | Partially Effective | Remove unnecessary administrative privileges and conduct periodic access reviews. |

## 4. Scenario-Based Mapping

### Scenario A — Microsoft 365 Account Compromise

**Risk:** Unauthorized Microsoft 365 access could expose sensitive information and enable account takeover.

**Relevant CSF functions:**

- **Govern:** Establish identity, access, and acceptable-use requirements.
- **Identify:** Identify privileged accounts, critical identities, and account-related risks.
- **Protect:** Enforce MFA, least privilege, conditional access, and secure authentication.
- **Detect:** Monitor authentication logs, anomalous sign-ins, and suspicious mailbox activity.
- **Respond:** Disable compromised accounts, revoke sessions, investigate activity, and communicate the incident.
- **Recover:** Restore account security, reset credentials, validate configurations, and document lessons learned.

**Priority:** Critical

### Scenario B — Critical Vendor Ransomware / Outage

**Risk:** A ransomware attack or prolonged outage affecting a critical third-party provider could interrupt MHTS operations and create security, availability, and compliance risks.

**Relevant CSF functions:**

- **Govern:** Establish third-party risk-management requirements and contractual security expectations.
- **Identify:** Identify critical vendors, dependencies, data flows, and concentration risks.
- **Protect:** Require appropriate vendor security controls, backups, access restrictions, and contingency arrangements.
- **Detect:** Monitor vendor security notifications and indicators of compromise affecting connected services.
- **Respond:** Activate incident-management and vendor-escalation procedures and assess business impact.
- **Recover:** Transition to contingency processes, restore affected services, validate vendor recovery, and conduct a post-incident review.

**Priority:** Critical

### Scenario C — Endpoint Ransomware

**Risk:** Ransomware infection on an employee endpoint could spread through the environment, disrupt operations, and expose organizational data.

**Relevant CSF functions:**

- **Identify:** Maintain endpoint inventory and identify critical systems and dependencies.
- **Protect:** Use endpoint protection, EDR, patch management, network segmentation, least privilege, and secure configuration baselines.
- **Detect:** Use EDR and centralized logging to identify malicious processes, encryption activity, and abnormal network behavior.
- **Respond:** Isolate affected endpoints, investigate the infection path, eradicate malware, and communicate incident status.
- **Recover:** Reimage or restore affected systems, validate backups, return systems to service, and document lessons learned.

**Priority:** Critical

## 5. Key GRC Observations

1. **Governance must connect cybersecurity activity to business risk.** The risk registers and security policies provide the foundation for prioritizing controls.
2. **Identity security is a major protection area** in a Microsoft 365-based hybrid workforce. MFA, least privilege, and monitoring are core safeguards.
3. **Third-party risk requires continuous oversight.** Critical vendors can introduce operational and cybersecurity dependencies outside direct organizational control.
4. **Detection depends on visibility.** Centralized logging, EDR, and meaningful alerting improve the ability to identify suspicious activity.
5. **Incident response should be exercised, not merely documented.** Tabletop exercises help validate roles, escalation paths, communications, and recovery decisions.
6. **Recovery requires tested procedures.** Backups and recovery plans should be periodically tested to establish that critical services can actually be restored.

## 6. Recommended Next Steps

### Priority 1 — Identity and Access

- Expand MFA coverage.
- Review privileged accounts.
- Implement or strengthen conditional-access controls.
- Conduct periodic access reviews.

### Priority 2 — Security Monitoring

- Centralize Microsoft 365, endpoint, AWS, and network security logs.
- Establish alerting and escalation procedures.
- Define log-retention requirements.

### Priority 3 — Third-Party Risk

- Classify vendors by criticality.
- Perform security assessments for critical vendors.
- Establish contractual security and incident-notification requirements.

### Priority 4 — Incident Response and Recovery

- Update the incident response plan.
- Conduct ransomware and account-compromise tabletop exercises.
- Test backup restoration and business-continuity procedures.

### Priority 5 — Continuous Governance

- Review the risk register quarterly.
- Track remediation activities to closure.
- Report significant cybersecurity risks and control gaps to appropriate leadership.

## 7. Conclusion

The NIST CSF 2.0 mapping demonstrates how MHTS can organize cybersecurity governance and controls around a common risk-management lifecycle. Cybersecurity is not limited to technical safeguards: governance, asset and risk understanding, identity protection, monitoring, incident response, third-party risk management, and recovery all contribute to organizational resilience.

This assessment should be treated as a working GRC document and updated as MHTS's technology environment, threat landscape, regulatory obligations, and business priorities change.
