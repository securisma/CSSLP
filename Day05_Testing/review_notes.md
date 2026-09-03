# Day 5 Review Notes – Secure Software Testing

## 1. Purpose of Security Testing

Security testing verifies that implemented controls behave as intended and that vulnerabilities are identified before deployment.  
It ensures requirements, design decisions, and implementation practices are validated through structured test activities.

Key goals:
- Identify security defects early.
- Validate security requirements and mitigations.
- Ensure controls are effective and complete.
- Support risk reduction and compliance.

---

## 2. Types of Security Testing

### Functional Security Testing
- Authentication and authorization tests.
- Input validation and sanitization tests.
- Session management tests.
- Error handling and logging tests.

### Non-Functional Security Testing
- Performance under attack (stress, load).
- Resilience and failover behavior.
- Security usability testing.

### Manual Testing
- Exploratory testing.
- Business logic abuse testing.
- Role-based access control validation.

### Automated Testing
- DAST (dynamic analysis).
- SAST (static analysis).
- Dependency scanning.
- API fuzzing.

---

## 3. Security Test Case Design

### Key Elements
- Objective: What the test validates.
- Preconditions: Required setup.
- Steps: Actions performed.
- Expected result: Secure behavior.
- Actual result: Logged during execution.

### Example Test Cases
Authentication:
- Missing token → expect 401.
- Expired token → expect 401.
- Invalid token → expect 401.

Authorization:
- User role accessing admin route → expect 403.
- Privilege escalation attempt → expect denial.

Input Validation:
- SQL injection payload → expect safe failure.
- Script injection → expect encoding or rejection.

Error Handling:
- Trigger error → expect generic message, detailed logs.

---

## 4. Dynamic Application Security Testing (DAST)

### Purpose
- Test running applications for vulnerabilities.
- Identify issues not visible in static code.
- Validate runtime behavior, configuration, and error handling.

### Typical Findings
- Missing or weak authentication.
- Broken access control.
- Injection vulnerabilities.
- Misconfigured headers.
- Information disclosure through error messages.

### ZAP Scan Notes
- Define target URLs.
- Configure context and authentication.
- Run active scan.
- Review findings and map them to requirements.

---

## 5. Vulnerability Tracking

### Key Fields
- Vulnerability ID
- Description
- Severity (Low, Medium, High, Critical)
- Status (Open, In Progress, Resolved)
- Owner
- Date discovered
- Date resolved

### Purpose
- Maintain visibility of security defects.
- Support remediation planning.
- Provide audit trail for compliance.

---

## 6. Relationship to Requirements and Architecture

Security testing validates:
- Requirements defined in Day 2.
- Threat mitigations identified in Day 3.
- Secure coding practices from Day 4.

Testing ensures the system behaves securely across all layers and trust boundaries.

---

## 7. Key Takeaways from Day 5
- Security testing is not only about finding bugs; it validates the entire SDLC.
- Test cases must be tied to requirements, threats, and controls.
- DAST complements SAST by identifying runtime issues.
- Vulnerability tracking is essential for governance and lifecycle management.
- Many CSSLP questions focus on selecting the correct testing method for a scenario.

---

## 8. Practice Question Notes
- Expect questions about choosing the right test type (SAST vs DAST vs manual).
- Many items test understanding of authentication, authorization, and input validation tests.
- Questions often emphasize traceability between requirements and test cases.
- Focus on lifecycle alignment: when testing should occur and why.

