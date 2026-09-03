# CSSLP Review Notes Book (Days 1–10)

This document consolidates all review notes from the 10‑day CSSLP preparation plan.  
Each day focuses on one domain or major competency area of the CSSLP exam.

---

# Day 1 – Secure Software Concepts

## 1. Core Security Principles
### CIA Triad
- Confidentiality: Prevent unauthorized access.
- Integrity: Prevent unauthorized modification.
- Availability: Ensure timely access to systems and data.

### AAA
- Authentication: Verify identity.
- Authorization: Determine access rights.
- Accounting: Track actions for auditing.

### Additional Principles
- Least Privilege
- Separation of Duties
- Defense-in-Depth
- Fail Secure
- Secure Defaults
- Complete Mediation

## 2. SDLC Security Integration
### Waterfall
- Security defined early, tested late.

### Agile
- Security embedded in each sprint.

### DevOps / DevSecOps
- Automated security in CI/CD pipelines.

## 3. Mapping Principles to SDLC Phases
- Requirements: Least privilege, secure defaults.
- Design: Threat modeling, separation of duties.
- Implementation: Input validation, secure coding.
- Testing: Verification of controls.
- Deployment/Operations: Hardening, monitoring.

## 4. Key Takeaways
- CSSLP emphasizes lifecycle thinking.
- Security must be planned early and validated continuously.

---

# Day 2 – Secure Software Requirements

## 1. Types of Requirements
### Functional
- Authentication
- Authorization
- Logging
- Input validation

### Non-Functional
- Encryption
- Availability
- Compliance
- Privacy

## 2. Compliance Requirements
- GDPR: Data minimization, breach notification.
- PCI-DSS: Encryption, segmentation.
- HIPAA: Access control, audit trails.

## 3. SRTM
- Requirement ID
- Source
- Threat
- Control
- Test case
- Status

## 4. Misuse/Abuse Cases
- Brute force login
- SQL injection
- Privilege escalation

## 5. Key Takeaways
- Requirements drive all downstream security activities.
- SRTM is central to CSSLP.

---

# Day 3 – Secure Architecture & Design

## 1. Architecture Fundamentals
- Reduce attack surface.
- Enforce trust boundaries.
- Apply layered controls.

## 2. STRIDE Threat Modeling
- Spoofing
- Tampering
- Repudiation
- Information Disclosure
- Denial of Service
- Elevation of Privilege

## 3. Data Flow Diagrams
- External entities
- Processes
- Data stores
- Data flows
- Trust boundaries

## 4. Secure Architecture Principles
- Least privilege
- Secure defaults
- Secrets vaults
- Centralized logging

## 5. Key Takeaways
- Architecture and design are heavily weighted in CSSLP.
- Threat modeling is essential.

---

# Day 4 – Secure Software Implementation

## 1. Secure Coding Principles
- Input validation
- Output encoding
- Error handling
- Session management
- Secrets management
- Parameterized queries

## 2. Common Insecure Patterns
- SQL injection
- Hardcoded secrets
- Unsafe deserialization
- Weak cryptography

## 3. Secure Alternatives
- Prepared statements
- Vault-based secrets
- Safe formats
- Modern algorithms

## 4. SAST
- Detects insecure coding patterns.
- Should be automated in CI/CD.

## 5. Key Takeaways
- Implementation is where many vulnerabilities originate.
- SAST and dependency hygiene are critical.

---

# Day 5 – Secure Software Testing

## 1. Purpose
- Validate controls.
- Identify vulnerabilities.
- Ensure requirements are met.

## 2. Types of Testing
### Functional
- AuthN/AuthZ
- Input validation
- Session management

### Non-Functional
- Performance under attack
- Resilience

### Automated
- DAST
- SAST
- Dependency scanning

## 3. Test Case Design
- Objective
- Preconditions
- Steps
- Expected result

## 4. DAST
- Tests running applications.
- Finds runtime issues.

## 5. Key Takeaways
- Testing validates the entire SDLC.
- Traceability between requirements and tests is essential.

---

# Day 6 – Secure Lifecycle Management

## 1. Governance and Roles
- Security architect
- Product owner
- Developers
- Testers
- Operations
- Compliance

## 2. Security Activities Across SDLC
- Requirements: SRTM
- Design: Threat modeling
- Implementation: Secure coding
- Testing: Security test cases
- Deployment: Hardening
- Operations: Monitoring
- Retirement: Secure disposal

## 3. CI/CD Security Gates
- Pre-commit: Secrets scanning
- Build: SAST, dependency scanning
- Test: DAST
- Deploy: IaC scanning
- Post-deploy: Monitoring

## 4. Metrics
- Vulnerability counts
- MTTR
- Test coverage
- Compliance adherence

## 5. Key Takeaways
- Lifecycle management is process-heavy.
- Governance and traceability matter.

---

# Day 7 – Deployment, Operations & Maintenance

## 1. Secure Deployment
- OS hardening
- Network segmentation
- TLS enforcement
- Least privilege service accounts

## 2. Secrets Management
- Vaults
- Rotation
- Access control

## 3. Logging and Monitoring
- Log auth events
- Log validation failures
- Centralized storage
- SIEM integration

## 4. Patch and Vulnerability Management
- Inventory
- Prioritization
- Testing
- Documentation

## 5. Incident Response
- Detect
- Contain
- Eradicate
- Recover
- Lessons learned

## 6. Key Takeaways
- Deployment security is continuous.
- Monitoring and IR are critical.

---

# Day 8 – Secure Software Supply Chain

## 1. SBOM
- Inventory of components
- Versions and licenses
- Transitive dependencies

## 2. Dependency Risks
- Outdated libraries
- Malicious packages
- Excessive dependency chains

## 3. Vendor Assessment
- Policies
- Patch practices
- IR capabilities
- SLAs

## 4. Build and Distribution Security
- Trusted build environments
- Code signing
- Secure artifact repositories

## 5. Key Takeaways
- Supply chain security is critical.
- SBOMs provide essential visibility.

---

# Day 9 – Mixed Practice & Weak Domain Analysis

## 1. Mixed Practice
- 100–125 questions recommended.

## 2. Categorizing Mistakes
- Domain
- Question type
- Root cause

## 3. Reinforcing Weak Domains
- Revisit notes
- Update diagrams
- Strengthen SRTM
- Expand test cases

## 4. Updating Artifacts
- Threat model
- Architecture diagrams
- SBOM
- IR playbook

## 5. Key Takeaways
- Mixed practice reveals readiness.
- Patterns indicate conceptual gaps.

---

# Day 10 – Final Review and Exam Preparation

## 1. Final Review
- SRTM
- Threat model
- DFDs
- Architecture diagrams
- Secure coding examples
- Test cases
- CI/CD gates
- SBOM
- IR playbook

## 2. Hardest Questions
- Revisit 10–15 difficult items.
- Document correct reasoning.

## 3. Exam Day Checklist
- Light review only.
- Prepare logistics.
- Ensure rest and clarity.

## 4. Exam Strategy
- Think like a security architect.
- Prioritize lifecycle alignment.
- Avoid technical rabbit holes.

## 5. Key Takeaways
- Day 10 is about readiness, not learning.
- Confidence and clarity matter more than volume.

---

# End of Review Notes Book
