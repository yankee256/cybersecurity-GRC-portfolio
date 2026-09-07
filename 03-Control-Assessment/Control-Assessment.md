# Control Assessment

## Project Overview

This control assessment evaluates selected cybersecurity controls associated with risks identified in the Midwest HealthTech Solutions (MHTS) simulated risk assessment.

**Organization:** Midwest HealthTech Solutions (MHTS)
**Industry:** Healthcare Technology
**Assessment Type:** Simulated Cybersecurity GRC Assessment
**Assessment Status:** Initial Control Assessment

> **Disclaimer:** Midwest HealthTech Solutions is a fictional organization created for this portfolio project. All findings, evidence, and assessment results are simulated and do not represent a real organization.

---

## Control Assessment Methodology

Controls are assessed using the following structure:

**Risk → Control → Control Objective → Evidence → Effectiveness → Gap → Recommendation**

### Control Effectiveness Ratings

| Rating              | Description                                                                                        |
| ------------------- | -------------------------------------------------------------------------------------------------- |
| Effective           | Control is consistently implemented, operating as intended, and supported by appropriate evidence. |
| Partially Effective | Control is implemented but gaps or inconsistent implementation reduce its effectiveness.           |
| Ineffective         | Control does not adequately achieve its intended security objective.                               |

---

# R-001 — Microsoft 365 Account Compromise

**Risk:** Microsoft 365 account compromise due to password reuse and lack of MFA.

### Control 1: Multi-Factor Authentication (MFA)

**Control Objective:**
Require users to authenticate using multiple factors to reduce the likelihood of unauthorized account access following credential compromise.

**Simulated Evidence:**

* Microsoft 365/Entra authentication configuration
* MFA enrollment reports
* Conditional Access policies
* Authentication logs

**Effectiveness:** **Ineffective**

**Control Gap:**
MFA is not consistently enforced for all users.

**Recommendation:**
Enforce MFA for all users and applications where technically feasible. Review MFA enrollment regularly and investigate accounts that remain outside the MFA requirement.

---

### Control 2: Strong Authentication & Session Controls

**Control Objective:**
Strengthen authentication requirements and limit unauthorized access through appropriate authentication and session-management policies.

**Simulated Evidence:**

* Conditional Access configuration
* Authentication policy settings
* Session-control configuration
* Authentication reports

**Effectiveness:** **Ineffective**

**Control Gap:**
Conditional Access and session controls are inconsistently configured across users and applications.

**Recommendation:**
Standardize authentication and session-control policies. Apply risk-based Conditional Access policies and periodically review authentication configurations.

---

### Control 3: Identity Monitoring, Logging & Automated Detection/Response

**Control Objective:**
Detect suspicious authentication activity and respond quickly to potential account compromise.

**Simulated Evidence:**

* Microsoft 365 sign-in logs
* Security alerts
* SIEM configuration
* Detection rules
* Incident-response procedures

**Effectiveness:** **Partially Effective**

**Control Gap:**
Authentication logs exist, but continuous centralized analysis and automated response capabilities are incomplete.

**Recommendation:**
Centralize identity and authentication logs in a security monitoring platform. Develop detection rules for suspicious sign-ins and automate appropriate responses to high-risk account activity.

---

# R-003 — Endpoint Ransomware

**Risk:** Ransomware affecting endpoints and systems accessible by employees.

### Control 4: Endpoint Protection

**Control Objective:**
Protect endpoints against malware, ransomware, and other malicious activity.

**Simulated Evidence:**

* Endpoint security console
* Antivirus status reports
* Endpoint compliance reports
* Malware detection records

**Effectiveness:** **Partially Effective**

**Control Gap:**
Endpoint security software is installed, but several laptops have outdated security software or signatures.

**Recommendation:**
Ensure endpoint security software and signatures remain current. Implement centralized monitoring and alerting for endpoints that fall out of compliance.

---

### Control 5: Endpoint Detection and Response (EDR)

**Control Objective:**
Detect, investigate, and respond to malicious activity occurring on endpoints.

**Simulated Evidence:**

* EDR deployment report
* Endpoint telemetry status
* Detection alerts
* Incident investigation records

**Effectiveness:** **Partially Effective**

**Control Gap:**
EDR is deployed on approximately 90% of endpoints, while 10% are not reporting telemetry.

**Recommendation:**
Achieve full EDR coverage across supported endpoints. Investigate devices that stop reporting telemetry and establish a defined remediation timeframe.

---

### Control 6: Patch Management

**Control Objective:**
Reduce vulnerabilities by ensuring operating systems and applications receive security patches within defined timeframes.

**Simulated Evidence:**

* Patch compliance reports
* Vulnerability scanner results
* Patch management dashboard
* Patch SLA reports

**Effectiveness:** **Partially Effective**

**Control Gap:**
Approximately 15% of laptops have critical patches that are more than 30 days overdue.

**Recommendation:**
Prioritize remediation of critical vulnerabilities. Establish patch-management SLAs and monitor compliance through centralized reporting.

---

### Control 7: Network Segmentation

**Control Objective:**
Limit the ability of attackers or malware to move laterally between systems and critical network environments.

**Simulated Evidence:**

* Network diagrams
* Firewall rules
* Access Control Lists (ACLs)
* Segmentation validation results

**Effectiveness:** **Partially Effective**

**Control Gap:**
Critical systems are segmented, but endpoints and several internal application servers share the same network segment.

**Recommendation:**
Improve network segmentation between user endpoints, application servers, and critical systems. Review firewall and ACL rules to restrict unnecessary communication between network zones.

---

# R-004 — Third-Party Security Risk

**Risk:** A third-party vendor has access to customer information without completing a cybersecurity assessment.

### Control 8: Third-Party Risk Assessment (TPRM)

**Control Objective:**
Identify and manage cybersecurity risks associated with vendors that have access to organizational systems or sensitive information.

**Simulated Evidence:**

* Vendor security questionnaire
* Vendor risk assessment
* Security certifications or reports
* Contractual security requirements
* Vendor assessment records

**Effectiveness:** **Partially Effective**

**Control Gap:**
A vendor handling customer information has not completed the organization's required cybersecurity assessment.

**Recommendation:**
Require completion of the vendor security assessment before granting or continuing sensitive access. Establish periodic reassessment requirements based on vendor risk.

---

# R-005 — Excessive Administrative Privileges

**Risk:** Employees have administrative privileges without a documented business requirement.

### Control 9: Least-Privilege Access / RBAC

**Control Objective:**
Ensure users receive only the level of access required to perform their assigned responsibilities.

**Simulated Evidence:**

* Access review reports
* Active Directory group memberships
* RBAC matrix
* Privileged account inventory
* Access approval records

**Effectiveness:** **Partially Effective**

**Control Gap:**
The organization has an access-control policy, but access reviews identified employees with unnecessary administrative privileges.

**Recommendation:**
Remove unnecessary administrative privileges. Implement role-based access control and conduct periodic access reviews for privileged accounts.

---

### Control 10: Zero Trust / Continuous Access Verification

**Control Objective:**
Continuously evaluate user, device, application, and access conditions rather than relying primarily on network location.

**Simulated Evidence:**

* Conditional Access policies
* Device compliance policies
* Application access policies
* Authentication and access logs

**Effectiveness:** **Partially Effective**

**Control Gap:**
Zero Trust controls are implemented for some critical applications, while other applications continue to rely primarily on network location.

**Recommendation:**
Expand Zero Trust principles across additional applications and systems. Require access decisions to consider identity, device security posture, application context, and other relevant risk signals.

---

# Control Assessment Summary

| Risk ID | Control                                  | Effectiveness       | Primary Gap                                      |
| ------- | ---------------------------------------- | ------------------- | ------------------------------------------------ |
| R-001   | Multi-Factor Authentication              | Ineffective         | MFA not consistently enforced                    |
| R-001   | Strong Authentication & Session Controls | Ineffective         | Inconsistent Conditional Access/session controls |
| R-001   | Identity Monitoring & Automated Response | Partially Effective | Limited centralized monitoring and automation    |
| R-003   | Endpoint Protection                      | Partially Effective | Outdated endpoint security                       |
| R-003   | EDR                                      | Partially Effective | 10% of endpoints lack telemetry                  |
| R-003   | Patch Management                         | Partially Effective | Critical patches overdue                         |
| R-003   | Network Segmentation                     | Partially Effective | Excessive shared network segments                |
| R-004   | Third-Party Risk Assessment              | Partially Effective | Vendor assessment incomplete                     |
| R-005   | Least Privilege / RBAC                   | Partially Effective | Excessive administrative privileges              |
| R-005   | Zero Trust                               | Partially Effective | Inconsistent implementation                      |

---

# Key Control Findings

The assessment identified the following primary control weaknesses:

1. **Identity security:** MFA and strong authentication controls require improvement.
2. **Security monitoring:** Identity monitoring and automated response capabilities are incomplete.
3. **Endpoint security:** Endpoint protection and EDR coverage require improvement.
4. **Vulnerability management:** Critical patches remain overdue on some endpoints.
5. **Network security:** Network segmentation does not sufficiently isolate all systems.
6. **Third-party risk:** A vendor with access to customer information has not completed the required security assessment.
7. **Privileged access:** Some employees maintain unnecessary administrative privileges.
8. **Zero Trust:** Access controls are not consistently applied across all applications.

---

# Recommended Priority Actions

Based on the control assessment, the recommended priorities are:

### Priority 1 — Strengthen Identity Security

* Enforce MFA.
* Standardize Conditional Access.
* Review privileged accounts.
* Improve identity monitoring.

### Priority 2 — Reduce Privileged Access

* Remove unnecessary administrative privileges.
* Implement RBAC.
* Conduct periodic access reviews.

### Priority 3 — Improve Endpoint Security

* Achieve full EDR coverage.
* Update endpoint security software.
* Remediate overdue critical patches.

### Priority 4 — Strengthen Third-Party Risk Management

* Complete vendor security assessments.
* Establish vendor security requirements.
* Perform periodic vendor reassessments.

### Priority 5 — Improve Network Segmentation

* Separate endpoints from critical application environments.
* Review firewall and ACL rules.
* Restrict unnecessary lateral communication.

---

## Assessment Conclusion

The simulated assessment indicates that MHTS has several cybersecurity controls in place, but many controls require improvement to consistently achieve their intended security objectives.

The highest-priority weaknesses involve identity security, privileged access, endpoint protection, vulnerability management, and third-party risk.

The next phase of the GRC assessment will map these controls to the **NIST Cybersecurity Framework (NIST CSF)** to identify the relevant cybersecurity functions, categories, and control relationships.
