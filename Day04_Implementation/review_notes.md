# Day 4 Review Notes – Secure Software Implementation

## 1. Secure Coding Principles

### Input Validation
- Validate all inputs on the server side.
- Reject unexpected types, formats, and ranges.
- Use allowlists instead of denylists.

### Output Encoding
- Encode output based on context (HTML, URL, JSON).
- Prevent XSS by sanitizing user-controlled data.

### Error Handling
- Do not reveal stack traces or internal details.
- Log errors securely without exposing sensitive data.
- Use generic user-facing error messages.

### Secure Session Management
- Use secure, HTTP-only cookies.
- Regenerate session IDs after authentication.
- Enforce session timeouts and inactivity limits.

### Secrets Management
- Never hardcode secrets in code.
- Store secrets in environment variables or vaults.
- Rotate keys and credentials regularly.

### Secure Database Access
- Use parameterized queries.
- Avoid dynamic SQL construction.
- Enforce least privilege on DB accounts.

---

## 2. Common Insecure Coding Patterns

### SQL Injection
- Building SQL queries with string concatenation.
- Using user input directly in queries.

### Hardcoded Secrets
- API keys, passwords, tokens inside source code.
- Credentials committed to version control.

### Unsafe Deserialization
- Deserializing untrusted input.
- Using insecure formats without validation.

### Insecure Cryptography
- Using outdated algorithms (MD5, SHA1).
- Implementing custom crypto logic.

### Improper Input Parsing
- Trusting client-side validation.
- Not sanitizing file uploads or command parameters.

---

## 3. Secure Alternatives

### SQL Injection Mitigation
- Use prepared statements.
- Bind parameters instead of concatenating strings.

### Secrets Handling
- Load secrets from secure storage.
- Use environment variables or vault APIs.

### Safe Deserialization
- Validate input before deserialization.
- Use safe formats (JSON) with strict schemas.

### Strong Cryptography
- Use modern algorithms (AES, SHA-256).
- Use vetted libraries instead of custom implementations.

---

## 4. Static Application Security Testing (SAST)

### Purpose
- Identify insecure coding patterns early.
- Automate detection of vulnerabilities.
- Integrate into CI/CD pipelines.

### Typical Findings
- Hardcoded credentials.
- SQL injection patterns.
- Unsafe file operations.
- Missing input validation.
- Weak cryptographic usage.

### Documentation
- Record findings in SAST reports.
- Map findings to requirements and threat model.
- Track remediation status.

---

## 5. Dependency and Supply Chain Considerations

### Risks
- Vulnerable third-party libraries.
- Outdated packages with known CVEs.
- Transitive dependencies introducing risk.

### Mitigation
- Use dependency scanning tools.
- Keep libraries updated.
- Prefer minimal dependency sets.

---

## 6. Key Takeaways from Day 4
- Implementation is where many vulnerabilities originate; secure coding is essential.
- SAST helps catch issues early and should be automated.
- Secure coding principles must align with requirements and architecture.
- Many CSSLP questions focus on identifying insecure patterns and selecting correct mitigations.
- Secure implementation is not only about code but also about dependency hygiene and secrets management.

---

## 7. Practice Question Notes
- Expect questions about secure vs insecure coding examples.
- Many items test understanding of input validation, output encoding, and secure database access.
- Questions often require identifying the best mitigation for a given insecure pattern.
- Focus on conceptual reasoning rather than language-specific syntax.

