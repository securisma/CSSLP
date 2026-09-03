# Day 2 Review Notes – Secure Software Requirements

## 1. Types of Security Requirements

### Functional Security Requirements
- Authentication mechanisms
- Authorization rules and role definitions
- Input validation and sanitization
- Logging and auditing behaviors
- Session management rules

### Non-Functional Security Requirements
- Encryption requirements (data at rest, data in transit)
- Performance impact of security controls
- Availability and resilience expectations
- Compliance obligations
- Privacy constraints and data minimization

---

## 2. Compliance-Driven Requirements

### GDPR
- Data minimization
- Purpose limitation
- Right to erasure
- Breach notification timelines

### PCI-DSS
- Encryption of cardholder data
- Network segmentation
- Strong access control policies
- Continuous monitoring and logging

### HIPAA (if applicable)
- Safeguards for PHI
- Access control and audit trails
- Integrity controls

Compliance requirements must be translated into actionable software requirements and mapped into the SRTM.

---

## 3. Security Requirements Traceability Matrix (SRTM)

### Key Columns
- Requirement ID
- Requirement description
- Source (business, compliance, threat model)
- Associated threat
- Mitigation or control
- Test case
- Verification status

### Purpose
- Ensures every security requirement is tracked
- Links requirements to threats and controls
- Provides visibility across the SDLC
- Supports auditing and governance

---

## 4. Misuse and Abuse Cases

### Example Structure
- Actor: Malicious user or insider
- Goal: What the attacker wants to achieve
- Method: How the attack is performed
- Impact: Business or technical consequences
- Mitigation: Controls to prevent or detect the attack

### Sample Cases
- Bypass authentication using brute force
- Inject malicious input into API parameters
- Access admin endpoints with user-level privileges

Misuse and abuse cases help refine and validate security requirements.

---

## 5. Key Takeaways from Day 2
- Requirements drive all downstream security activities; missing requirements create blind spots.
- Non-functional requirements are often more critical than functional ones in CSSLP.
- Compliance obligations must be converted into explicit, testable requirements.
- SRTM is central to CSSLP thinking and appears across multiple domains.
- Misuse and abuse cases strengthen requirements and threat modeling.

---

## 6. Practice Question Notes
- Many questions focus on distinguishing functional vs non-functional requirements.
- Expect scenarios where compliance must be translated into software requirements.
- SRTM questions often test understanding of traceability and lifecycle alignment.
- Requirements questions frequently emphasize early-phase security involvement.

