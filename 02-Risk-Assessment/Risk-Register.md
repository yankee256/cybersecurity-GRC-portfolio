# Cybersecurity GRC Risk Register

## Project Overview

This risk register is part of a simulated cybersecurity Governance, Risk, and Compliance (GRC) assessment for **Midwest HealthTech Solutions (MHTS)**, a fictional healthcare technology organization.

The assessment identifies cybersecurity risks, evaluates likelihood and impact, and recommends appropriate risk treatment and remediation activities.

> **Note:** This is a fictional portfolio project created for educational and professional development purposes. No real company, customer, or confidential information is represented.

---

## Risk Scoring Methodology

Risk is evaluated using:

**Risk Score = Likelihood × Impact**

### Likelihood Scale

| Score | Rating         | Description                     |
| ----: | -------------- | ------------------------------- |
|     1 | Rare           | Highly unlikely to occur        |
|     2 | Unlikely       | Could occur but is not expected |
|     3 | Possible       | Could reasonably occur          |
|     4 | Likely         | Expected to occur               |
|     5 | Almost Certain | Very likely to occur            |

### Impact Scale

| Score | Rating        | Description                                              |
| ----: | ------------- | -------------------------------------------------------- |
|     1 | Insignificant | Minimal operational impact                               |
|     2 | Minor         | Limited disruption or loss                               |
|     3 | Moderate      | Noticeable business impact                               |
|     4 | Major         | Significant operational or financial impact              |
|     5 | Severe        | Critical business, financial, regulatory, or data impact |

### Risk Rating

| Score | Rating   |
| ----: | -------- |
|   1–4 | Low      |
|   5–9 | Medium   |
| 10–16 | High     |
| 17–25 | Critical |

---

# Risk Register

| ID    | Risk                                                                                       | Asset / Area                | Likelihood | Impact | Score | Rating   | Treatment |
| ----- | ------------------------------------------------------------------------------------------ | --------------------------- | ---------: | -----: | ----: | -------- | --------- |
| R-001 | Microsoft 365 account compromise due to password reuse and lack of MFA                     | Microsoft 365 / Identity    |          4 |      5 |    20 | Critical | Mitigate  |
| R-002 | Critical vendor ransomware causing service disruption                                      | Cloud Vendor                |          5 |      5 |    25 | Critical | Mitigate  |
| R-003 | Endpoint ransomware affecting systems accessible by the employee                           | Endpoint / Internal Systems |          4 |      5 |    20 | Critical | Mitigate  |
| R-004 | Third-party vendor has access to customer information without a security assessment        | Third-Party Risk            |          3 |      5 |    15 | High     | Mitigate  |
| R-005 | Excessive administrative privileges assigned to an employee without a business requirement | Active Directory / IAM      |          5 |      5 |    25 | Critical | Mitigate  |

---

# Detailed Risk Assessments

## R-001 — Microsoft 365 Account Compromise

**Threat:** Credential theft and account takeover

**Vulnerability:** Password reuse and lack of multi-factor authentication (MFA)

**Potential Impact:** Unauthorized access to email, business information, cloud resources, and sensitive organizational data.

**Risk Score:** 20/25

**Rating:** Critical

**Recommended Treatment:** Mitigate

**Recommended Remediation:**

* Enforce MFA for all Microsoft 365 accounts.
* Implement conditional access policies.
* Strengthen authentication requirements.
* Conduct periodic identity and access reviews.
* Educate employees about password reuse and credential phishing.

---

## R-002 — Critical Vendor Ransomware

**Threat:** Ransomware attack against a critical third-party provider

**Vulnerability:** Dependency on a critical vendor and potential weaknesses in third-party security controls.

**Potential Impact:** Service interruption, operational disruption, financial loss, and potential data exposure.

**Risk Score:** 25/25

**Rating:** Critical

**Recommended Treatment:** Mitigate

**Recommended Remediation:**

* Conduct security assessments of critical vendors.
* Establish contractual cybersecurity requirements.
* Require timely security incident notification.
* Evaluate vendor business continuity and disaster recovery capabilities.
* Develop contingency plans for critical third-party services.

---

## R-003 — Endpoint Ransomware

**Threat:** Malware or ransomware

**Vulnerability:** Compromised endpoint with access to internal systems

**Potential Impact:** Data encryption, business disruption, credential theft, and lateral movement.

**Risk Score:** 20/25

**Rating:** Critical

**Recommended Treatment:** Mitigate

**Recommended Remediation:**

* Deploy endpoint detection and response (EDR).
* Maintain current endpoint security software.
* Apply security patches promptly.
* Enforce least privilege.
* Segment critical network resources.
* Maintain tested backups.
* Review incident response procedures.

---

## R-004 — Third-Party Data Security

**Threat:** Vendor compromise or unauthorized access

**Vulnerability:** Vendor has access to customer information but has not completed a cybersecurity assessment.

**Potential Impact:** Unauthorized disclosure of customer information, regulatory exposure, reputational damage, and financial loss.

**Risk Score:** 15/25

**Rating:** High

**Recommended Treatment:** Mitigate

**Recommended Remediation:**

* Perform a formal third-party security assessment.
* Review vendor security policies and controls.
* Evaluate access privileges.
* Establish contractual security requirements.
* Require appropriate incident notification procedures.
* Reassess the vendor periodically.

---

## R-005 — Excessive Administrative Privileges

**Threat:** Account compromise or insider misuse

**Vulnerability:** Employee has administrative privileges that are not required for their job responsibilities.

**Potential Impact:** Unauthorized system changes, privilege escalation, lateral movement, data access, or broader environment compromise.

**Risk Score:** 25/25

**Rating:** Critical

**Recommended Treatment:** Mitigate

**Recommended Remediation:**

* Remove unnecessary administrative privileges.
* Implement least privilege.
* Use role-based access control (RBAC).
* Establish privileged access management (PAM).
* Conduct periodic access reviews.
* Require approval for privileged access.

---

# Risk Treatment Strategy

The primary treatment strategy for the identified risks is **mitigation**.

Risk mitigation will focus on reducing either the likelihood of occurrence, the potential impact, or both through appropriate security controls and governance processes.

Priority should initially be given to:

1. Excessive administrative privileges
2. Critical third-party/vendor risk
3. Microsoft 365 identity security
4. Endpoint ransomware protection
5. Third-party data security assessment

---

## Assessment Status

**Project Type:** Simulated GRC Portfolio Project

**Assessment Status:** Initial Risk Assessment

**Next Phase:** Security Control Assessment and NIST CSF Mapping
