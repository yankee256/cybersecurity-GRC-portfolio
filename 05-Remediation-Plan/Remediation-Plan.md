## R-001 — Microsoft 365 Account Compromise

| Field | Details |
|---|---|
| Finding | MFA and authentication controls are inconsistent |
| Priority | Critical |
| Owner | IAM / Security |
| Target | 30 days |
| Status | Open |
| Residual Risk | Medium |

### Remediation
1. Enforce MFA.
2. Standardize Conditional Access.
3. Review privileged accounts.
4. Disable unnecessary legacy authentication.
5. Establish periodic access reviews.

### Evidence
- MFA enrollment report
- Conditional Access configuration
- Privileged account review
- Authentication logs

### Validation
GRC verifies that MFA is consistently enforced and high-risk authentication events are monitored.

### Closure Criteria
Close when the controls are implemented consistently and supporting evidence confirms effectiveness.
