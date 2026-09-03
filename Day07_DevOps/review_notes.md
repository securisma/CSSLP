# Day 7 Review Notes – Secure Deployment, Operations & Maintenance

## 1. Purpose of Secure Deployment and Operations

Secure deployment and operations ensure that the software, once released, continues to run securely in its target environment.  
This phase focuses on configuration, hardening, monitoring, patching, and incident response.

Key goals:
- Deploy systems with secure configurations.
- Maintain continuous monitoring and logging.
- Protect secrets and sensitive operational data.
- Respond effectively to incidents.
- Ensure long-term security through maintenance and updates.

---

## 2. Secure Deployment Practices

### Environment Hardening
- Disable unnecessary services and ports.
- Enforce secure OS and container baselines.
- Apply least privilege to service accounts.
- Use secure configurations for web servers, databases, and APIs.

### Network Security
- Enforce segmentation and isolation.
- Use firewalls and allowlists.
- Apply TLS everywhere.
- Validate certificates and enforce strong cipher suites.

### Secrets and Configuration Management
- Store secrets in vaults or secure key stores.
- Avoid embedding secrets in code or config files.
- Rotate keys and credentials regularly.
- Enforce strict access controls for secret retrieval.

### Infrastructure as Code (IaC)
- Use IaC templates for consistent deployments.
- Scan IaC for misconfigurations before deployment.
- Track configuration drift across environments.

---

## 3. Logging and Monitoring

### Logging Requirements
- Log authentication and authorization events.
- Log input validation failures.
- Log configuration changes.
- Log access to sensitive data.
- Ensure logs are tamper-resistant.

### Monitoring Requirements
- Monitor system health and performance.
- Monitor security events and anomalies.
- Use alerting thresholds for suspicious activity.
- Integrate logs into SIEM platforms.

### Common Issues
- Missing logs for critical events.
- Excessive logging of sensitive data.
- Lack of centralized log storage.
- No alerting on high-risk events.

---

## 4. Patch and Vulnerability Management

### Patch Management
- Maintain an inventory of software and dependencies.
- Apply patches based on severity and exposure.
- Test patches before deployment.
- Document patch cycles and exceptions.

### Vulnerability Management
- Continuously scan systems and dependencies.
- Prioritize vulnerabilities based on risk.
- Track remediation in a vulnerability management system.
- Validate fixes through retesting.

---

## 5. Incident Response (IR)

### IR Phases
1. Detect  
2. Contain  
3. Eradicate  
4. Recover  
5. Lessons Learned

### Key Components
- Clear roles and responsibilities.
- Communication plan for internal and external stakeholders.
- Evidence collection and preservation.
- Post-incident review and improvement plan.

### Common IR Challenges
- Lack of clear ownership.
- Missing logs or insufficient visibility.
- Slow containment due to unclear procedures.

---

## 6. Maintenance and Continuous Improvement

### Maintenance Activities
- Regular patching and updates.
- Reviewing logs and alerts.
- Updating configurations and baselines.
- Rotating secrets and credentials.
- Reviewing access rights and privileges.

### Continuous Improvement
- Update threat models based on new findings.
- Improve monitoring rules.
- Enhance deployment pipelines.
- Refine IR playbooks.

---

## 7. Key Takeaways from Day 7
- Deployment and operations are critical for long-term security.
- Hardening, secrets management, and monitoring form the foundation of secure operations.
- Incident response must be well-defined, practiced, and continuously improved.
- Many CSSLP questions focus on operational controls, logging, monitoring, and patching.
- Secure deployment is not a one-time activity; it requires continuous maintenance.

---

## 8. Practice Question Notes
- Expect questions about logging, monitoring, and incident response workflows.
- Many items test understanding of secure configuration and environment hardening.
- Questions often emphasize operational responsibilities and lifecycle alignment.
- Focus on process, governance, and continuous improvement rather than technical exploitation.

