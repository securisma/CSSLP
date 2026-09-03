# CSSLP Cheat Sheet

A compact reference covering the core concepts, lifecycle activities, and exam-critical knowledge for the Certified Secure Software Lifecycle Professional (CSSLP).

---

# 1. Security Principles

## CIA
- Confidentiality: Prevent unauthorized access.
- Integrity: Prevent unauthorized modification.
- Availability: Ensure timely access.

## AAA
- Authentication: Verify identity.
- Authorization: Determine access rights.
- Accounting: Track actions.

## Core Principles
- Least Privilege
- Separation of Duties
- Defense-in-Depth
- Fail Secure
- Secure Defaults
- Complete Mediation
- Open Design
- Economy of Mechanism

---

# 2. SDLC Security Activities

## Requirements
- Identify functional and non-functional security requirements.
- Map compliance obligations.
- Build SRTM.

## Design
- Threat modeling (STRIDE).
- Architecture diagrams and trust boundaries.
- Select security patterns and controls.

## Implementation
- Secure coding practices.
- Secrets management.
- SAST and dependency scanning.

## Testing
- Security test cases.
- DAST and manual testing.
- Validate mitigations.

## Deployment
- Hardening.
- Secure configurations.
- IaC scanning.

## Operations
- Monitoring and logging.
- Patch and vulnerability management.
- Incident response.

## Retirement
- Secure data disposal.
- Access removal.
- Documentation archiving.

---

# 3. STRIDE Threat Modeling

- Spoofing → Authentication
- Tampering → Integrity controls
- Repudiation → Logging and auditing
- Information Disclosure → Encryption
- Denial of Service → Resource limits
- Elevation of Privilege → Authorization

---

# 4. SRTM (Security Requirements Traceability Matrix)

## Columns
- Requirement ID
- Description
- Source (business, compliance, threat)
- Threat
- Control
- Test case
- Status

## Purpose
- Ensures traceability across SDLC.
- Links requirements to threats and controls.
- Supports auditing and governance.

---

# 5. Secure Coding Essentials

## Input Validation
- Server-side validation.
- Allowlists preferred.

## Output Encoding
- Encode based on context (HTML, URL, JSON).

## Error Handling
- No sensitive data in messages.
- Log securely.

## Database Security
- Parameterized queries.
- Least privilege DB accounts.

## Secrets Management
- No hardcoded secrets.
- Use vaults or environment variables.

## Cryptography
- Use modern algorithms (AES, SHA-256).
- Avoid custom crypto.

---

# 6. Security Testing

## Functional
- AuthN/AuthZ
- Input validation
- Session management

## Non-Functional
- Performance under attack
- Resilience

## Automated
- SAST
- DAST
- Dependency scanning

## Test Case Structure
- Objective
- Preconditions
- Steps
- Expected result

---

# 7. CI/CD Security Gates

## Pre-Commit
- Secrets scanning
- Secure linting

## Build
- SAST
- Dependency scanning

## Test
- DAST
- API security tests

## Deploy
- IaC scanning
- Configuration validation

## Post-Deploy
- Monitoring
- Log analysis

---

# 8. Logging & Monitoring

## Logging
- Auth events
- Validation failures
- Config changes
- Sensitive data access

## Monitoring
- Security events
- System health
- Anomaly detection
- SIEM integration

---

# 9. Incident Response

## Phases
1. Detect  
2. Contain  
3. Eradicate  
4. Recover  
5. Lessons Learned

## Requirements
- Clear roles
- Communication plan
- Evidence preservation
- Post-incident improvements

---

# 10. Supply Chain Security

## SBOM
- Inventory of components
- Versions and licenses
- Transitive dependencies

## Dependency Risks
- Outdated libraries
- Malicious packages
- Excessive dependency chains

## Vendor Assessment
- Policies
- Patch practices
- IR capabilities
- SLAs

## Build Security
- Trusted build environments
- Code signing
- Secure artifact repositories

---

# 11. Common Exam Pitfalls

- Confusing lifecycle phases.
- Over-focusing on technical details.
- Ignoring governance and roles.
- Misinterpreting requirements vs design vs implementation.
- Forgetting traceability across SDLC.

---

# 12. Exam Strategy

- Think like a security architect.
- Prioritize lifecycle alignment.
- Choose answers emphasizing governance, process, and traceability.
- Avoid overly technical interpretations unless clearly required.

---

# End of CSSLP Cheat Sheet
