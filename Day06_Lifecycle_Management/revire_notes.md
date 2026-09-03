# Day 6 Review Notes – Secure Software Lifecycle Management

## 1. Purpose of Secure Lifecycle Management

Secure lifecycle management ensures that security is embedded across every phase of the SDLC.  
It focuses on governance, roles, processes, metrics, and continuous improvement rather than technical controls.

Key goals:
- Integrate security activities into all SDLC phases.
- Ensure traceability from requirements to deployment.
- Establish governance and accountability.
- Maintain security posture throughout the software lifecycle.

---

## 2. Governance and Roles

### Common Roles
- Security Architect: Defines security design and controls.
- Product Owner: Ensures security requirements align with business needs.
- Developers: Implement secure coding practices.
- Testers: Validate security controls.
- Operations Team: Maintain secure deployments and monitoring.
- Compliance/Legal: Ensure regulatory alignment.

### Governance Activities
- Policy creation and enforcement.
- Risk management and prioritization.
- Change management and approval workflows.
- Documentation and audit readiness.

---

## 3. Security Activities Across the SDLC

### Requirements Phase
- Identify security requirements.
- Map compliance obligations.
- Create SRTM entries.

### Design Phase
- Perform threat modeling.
- Define architecture and trust boundaries.
- Select security patterns and controls.

### Implementation Phase
- Apply secure coding practices.
- Run SAST and dependency scanning.
- Enforce secrets management.

### Testing Phase
- Execute security test cases.
- Run DAST and manual tests.
- Validate mitigations and controls.

### Deployment Phase
- Apply hardening and configuration controls.
- Validate environment security.
- Ensure secure CI/CD pipelines.

### Operations Phase
- Monitor logs and alerts.
- Patch vulnerabilities.
- Maintain incident response readiness.

### Retirement Phase
- Secure data disposal.
- Remove access and credentials.
- Archive documentation.

---

## 4. CI/CD Security Gates

### Pre-Commit
- Secrets scanning
- Linting for secure coding patterns

### Build Stage
- SAST
- Dependency scanning

### Test Stage
- DAST
- API security tests

### Deploy Stage
- Infrastructure-as-code scanning
- Configuration validation

### Post-Deploy
- Runtime monitoring
- Log analysis

Security gates ensure that insecure code or configurations cannot progress through the pipeline.

---

## 5. Metrics and Maturity Models

### Common Security Metrics
- Number of vulnerabilities by severity
- Mean time to remediate (MTTR)
- Coverage of security test cases
- Compliance adherence
- SAST/DAST pass rates
- Dependency risk scores

### Maturity Models
- CMMI
- BSIMM
- SAMM

Purpose:
- Assess current security posture.
- Identify gaps.
- Plan improvements.

---

## 6. Change and Configuration Management

### Change Management
- Document changes.
- Assess security impact.
- Obtain approvals.
- Track version history.

### Configuration Management
- Maintain secure baseline configurations.
- Use IaC for consistency.
- Track configuration drift.

---

## 7. Key Takeaways from Day 6
- Lifecycle management is process-heavy and central to CSSLP.
- Governance, roles, and metrics matter as much as technical controls.
- CI/CD security gates enforce continuous security.
- Security must be traceable across all SDLC phases.
- Many exam questions focus on “when” and “who” rather than “how.”

---

## 8. Practice Question Notes
- Expect questions about selecting the correct lifecycle phase for a security activity.
- Many items test understanding of governance, roles, and responsibilities.
- CI/CD security gate questions are common.
- Focus on lifecycle alignment and traceability rather than technical depth.

