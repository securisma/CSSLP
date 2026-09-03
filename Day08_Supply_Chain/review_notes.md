# Day 8 Review Notes – Secure Software Supply Chain

## 1. Purpose of Supply Chain Security

Supply chain security ensures that all third-party components, libraries, services, and tools used in the software lifecycle are trustworthy, maintained, and free from known vulnerabilities.

Key goals:
- Identify and manage risks introduced by external dependencies.
- Maintain visibility into all components through SBOMs.
- Validate vendor security posture.
- Prevent compromised or malicious packages from entering the system.

---

## 2. Software Bill of Materials (SBOM)

### What an SBOM Provides
- Complete inventory of all software components.
- Versions, licenses, and dependency relationships.
- Visibility into transitive dependencies.
- Ability to quickly identify vulnerable components.

### Common SBOM Formats
- CycloneDX
- SPDX

### SBOM Tools
- Syft
- CycloneDX CLI

### SBOM Use Cases
- Vulnerability management
- Compliance reporting
- Incident response
- Dependency audits

---

## 3. Dependency Risk Analysis

### Common Risks
- Outdated libraries with known CVEs.
- Unmaintained or abandoned packages.
- Malicious or compromised packages.
- Excessive dependency chains.
- License incompatibilities.

### Mitigation Strategies
- Regular dependency scanning.
- Pinning versions to known-good releases.
- Using minimal dependency sets.
- Reviewing package maintainers and update frequency.
- Removing unused or deprecated libraries.

### Risk Scoring Factors
- CVSS score of vulnerabilities.
- Exposure (public-facing vs internal).
- Criticality of the component.
- Update frequency and maintenance status.

---

## 4. Vendor and Third-Party Assessment

### Vendor Assessment Criteria
- Security policies and certifications.
- Patch and update practices.
- Incident response capabilities.
- Data protection and privacy controls.
- SLA and uptime guarantees.

### Third-Party Service Risks
- API reliability and security.
- Data sharing and retention policies.
- Authentication and authorization mechanisms.
- Integration security (tokens, secrets, certificates).

### Contractual Controls
- Security requirements in contracts.
- Breach notification timelines.
- Right to audit clauses.
- Data handling and deletion requirements.

---

## 5. Secure Build and Distribution Practices

### Build Security
- Use trusted build environments.
- Enforce code signing for artifacts.
- Validate integrity of build outputs.
- Protect CI/CD pipelines from tampering.

### Distribution Security
- Use secure artifact repositories.
- Enforce access controls on package registries.
- Validate signatures before deployment.

---

## 6. Threats to the Software Supply Chain

### Common Threats
- Dependency hijacking (typosquatting, namespace attacks).
- Malicious package updates.
- Compromised build systems.
- Poisoned CI/CD pipelines.
- Insider threats in third-party vendors.

### Real-World Examples
- Dependency confusion attacks.
- Compromised NPM/PyPI packages.
- Build system compromises leading to malicious updates.

---

## 7. Key Takeaways from Day 8
- Supply chain security is one of the most important CSSLP domains due to modern dependency-heavy development.
- SBOMs provide essential visibility into all components and dependencies.
- Dependency risk analysis must be continuous, not one-time.
- Vendor assessments ensure external services meet security expectations.
- Build and distribution security protect against tampering and malicious updates.
- Many CSSLP questions focus on identifying supply chain risks and selecting appropriate mitigations.

---

## 8. Practice Question Notes
- Expect questions about SBOM purpose and usage.
- Many items test understanding of dependency risks and mitigation strategies.
- Vendor assessment questions often emphasize governance and contractual controls.
- Focus on lifecycle alignment: supply chain security spans requirements, design, implementation, and operations.

