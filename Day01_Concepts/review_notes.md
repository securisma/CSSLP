# Day 1 Review Notes – Secure Software Concepts

## 1. Core Security Principles

### CIA Triad
- Confidentiality: Protect data from unauthorized access.
- Integrity: Ensure data is accurate, consistent, and unaltered.
- Availability: Ensure systems and data are accessible when needed.

### AAA
- Authentication: Verifying identity.
- Authorization: Determining access rights.
- Accounting: Tracking actions for auditing and non-repudiation.

### Additional Principles
- Least Privilege: Users and processes get only the minimum access required.
- Separation of Duties: Split critical tasks across multiple roles.
- Defense-in-Depth: Multiple layers of security controls.
- Fail Secure: Systems should fail in a secure state.
- Secure Defaults: Default configurations should be secure.
- Complete Mediation: Every access request must be checked.

---

## 2. SDLC Security Integration

### Waterfall
- Security requirements defined early.
- Security testing occurs late.
- High risk of late discovery of issues.

### Agile
- Security activities embedded in each sprint.
- Continuous threat modeling and code review.
- Frequent releases require automated security checks.

### DevOps / DevSecOps
- Security integrated into CI/CD pipelines.
- Automated SAST, DAST, dependency scanning.
- Shared responsibility between development and operations.

---

## 3. Mapping Principles to SDLC Phases

### Requirements Phase
- Least privilege
- Secure defaults
- Compliance-driven requirements

### Design Phase
- Defense-in-depth
- Separation of duties
- Threat modeling

### Implementation Phase
- Input validation
- Output encoding
- Secure error handling

### Testing Phase
- Complete mediation
- Verification of controls
- Security test cases

### Deployment & Operations
- Hardening
- Monitoring and logging
- Incident response

---

## 4. Key Takeaways from Day 1
- CSSLP is heavily focused on concepts and lifecycle thinking, not deep technical exploitation.
- Security must be planned early and validated continuously.
- Principles like least privilege and defense-in-depth appear across multiple domains.
- Understanding how security fits into SDLC models is essential for exam questions.

---

## 5. Practice Question Notes
- Questions often test conceptual differences (e.g., authentication vs authorization).
- Many items focus on governance and process rather than technical implementation.
- Pay attention to “best phase to perform X” type questions.
- Avoid technical rabbit holes; think like a security architect.

