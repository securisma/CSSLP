# Day 3 Review Notes – Secure Software Architecture & Design

## 1. Architecture Fundamentals

### Security Architecture Goals
- Reduce attack surface.
- Enforce trust boundaries.
- Ensure secure data flows.
- Apply layered controls (technical, administrative, physical).

### Common Architecture Patterns
- Layered architecture (presentation, business logic, data).
- Microservices architecture (service isolation, API gateways).
- Zero Trust architecture (continuous verification, least privilege).
- Client-server architecture (clear separation of responsibilities).

---

## 2. Threat Modeling (STRIDE)

### STRIDE Categories
- Spoofing: Impersonating identities.
- Tampering: Modifying data or code.
- Repudiation: Denying actions due to lack of logging.
- Information Disclosure: Unauthorized data exposure.
- Denial of Service: Making services unavailable.
- Elevation of Privilege: Gaining higher access than intended.

### Threat Modeling Steps
1. Define system scope and assets.
2. Create data flow diagrams (DFDs).
3. Identify trust boundaries.
4. Apply STRIDE to each component and data flow.
5. Document mitigations and residual risks.

### Common Mitigations
- MFA, strong authentication.
- Input validation and output encoding.
- Encryption in transit and at rest.
- Logging and auditing.
- Rate limiting and resource isolation.
- RBAC and privilege separation.

---

## 3. Data Flow Diagrams (DFDs)

### Key Elements
- External entities (users, third-party services).
- Processes (API, authentication service).
- Data stores (databases, caches).
- Data flows (HTTP requests, DB queries).
- Trust boundaries (network segments, privilege zones).

### Purpose
- Visualize how data moves through the system.
- Identify where threats apply.
- Support STRIDE analysis.

---

## 4. Secure Architecture Design

### Core Design Principles
- Minimize attack surface.
- Enforce least privilege at every layer.
- Use secure defaults.
- Separate duties across components.
- Protect secrets using vaults or HSMs.
- Implement centralized logging and monitoring.

### Typical Components in Secure Architecture
- API gateway for request filtering.
- Authentication service for identity management.
- Application service for business logic.
- Database with strict access controls.
- Secrets vault for key and credential storage.
- Logging pipeline for audit trails.

---

## 5. Trust Boundaries

### Examples
- User → Web application boundary.
- Web application → API boundary.
- API → Database boundary.
- Internal → External service boundary.

### Why They Matter
- Threats often occur at boundaries.
- Controls must be applied where trust changes.
- Helps determine where encryption, validation, and authentication are required.

---

## 6. Key Takeaways from Day 3
- Architecture and design are heavily weighted in CSSLP.
- Threat modeling is a recurring theme across multiple domains.
- DFDs are essential for identifying threats and designing mitigations.
- Secure architecture requires layered controls and clear trust boundaries.
- Many exam questions focus on selecting the correct mitigation for a given threat.

---

## 7. Practice Question Notes
- Expect scenario-based questions involving STRIDE.
- Many questions test understanding of trust boundaries and data flows.
- Architecture questions often emphasize secure design choices rather than implementation details.
- Focus on reasoning: “Which control best mitigates this threat?” rather than technical specifics.

