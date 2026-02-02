# Security Policy

**Last Updated:** February 2, 2026  
**Repository:** git-mcp  
**Organization:** RemyLoveLogicAI  
**Compliance Standards:** SOC2, ISO 27001, PCI-DSS

---

## 1. Vulnerability Disclosure Process

We take the security of git-mcp seriously. If you discover a security vulnerability, we appreciate your help in disclosing it to us in a responsible manner.

### Reporting a Vulnerability

**DO NOT** create public GitHub issues for security vulnerabilities. Instead, please follow these steps:

1. **Email Security Team:** Send details to `security@lovelogicai.com`
2. **Include Details:**
   - Type of vulnerability
   - Full paths of source file(s) related to the vulnerability
   - Location of the affected source code (tag/branch/commit or direct URL)
   - Step-by-step instructions to reproduce the issue
   - Proof-of-concept or exploit code (if possible)
   - Impact of the vulnerability, including how an attacker might exploit it

3. **Encrypted Communication:** For sensitive information, use our PGP key available upon request
4. **Response Time:** You will receive an acknowledgment within 48 hours
5. **Status Updates:** We will keep you informed about the progress toward a fix

### What to Expect

- **Acknowledgment:** Within 48 business hours
- **Initial Assessment:** Within 5 business days
- **Status Updates:** Every 7 days until resolution
- **Resolution Timeline:** Critical vulnerabilities within 30 days; others based on severity

---

## 2. Security Incident Reporting Procedures

### Internal Incident Response

When a security incident is detected:

1. **Immediate Containment:** Isolate affected systems/components
2. **Incident Classification:** Assess severity (Critical, High, Medium, Low)
3. **Notification:** Alert security team and stakeholders
4. **Investigation:** Root cause analysis and impact assessment
5. **Remediation:** Deploy patches or mitigations
6. **Documentation:** Record all actions in incident log
7. **Post-Incident Review:** Conduct retrospective within 7 days

### Severity Levels

| Severity | Description | Response Time |
|----------|-------------|---------------|
| **Critical** | Actively exploited, data breach, system compromise | Immediate (< 4 hours) |
| **High** | Significant security risk, potential for exploitation | 24 hours |
| **Medium** | Moderate risk, requires authentication or special conditions | 7 days |
| **Low** | Minor risk, limited impact | 30 days |

### User Reporting

If you believe your data has been compromised or notice suspicious activity:

- **Email:** security@lovelogicai.com
- **Subject Line:** "SECURITY INCIDENT - git-mcp"
- **Include:** Account details, timestamp, description of the issue

---

## 3. Responsible Disclosure Policy

We are committed to working with security researchers and the community to verify and address security vulnerabilities.

### Safe Harbor

We support safe harbor for security researchers who:

- Make a good faith effort to avoid privacy violations, data destruction, and service interruption
- Only interact with accounts you own or with explicit permission from the account holder
- Do not exploit vulnerabilities beyond the minimum necessary to confirm existence
- Report vulnerabilities promptly after discovery
- Provide reasonable time to address issues before public disclosure

**We will not pursue legal action** against researchers who comply with this policy.

### Scope

**In Scope:**
- git-mcp application code
- Authentication and authorization mechanisms
- Data handling and storage
- API endpoints and integrations
- Dependencies and third-party components
- Git operations and MCP protocol implementation

**Out of Scope:**
- Social engineering attacks
- Denial of Service (DoS) attacks
- Physical attacks against infrastructure
- Third-party services not directly controlled by this project

### Rules of Engagement

- Do not access, modify, or delete data belonging to others
- Do not perform attacks that could harm system reliability or performance
- Do not use automated scanners without prior approval
- Respect user privacy at all times
- Only test against systems you have permission to access

### Recognition

Researchers who responsibly disclose valid vulnerabilities will be:
- Acknowledged in our security advisories (with permission)
- Listed in our Hall of Fame (optional)
- Eligible for bounty rewards (if program established)

---

## 4. Security Contact Information

### Primary Security Contact

**Email:** security@lovelogicai.com  
**Response Time:** Within 48 hours  
**PGP Key:** Available upon request via email

### Alternative Contacts

**Repository Maintainer:** @RemyLoveLogicAI  
**GitHub Security Advisories:** https://github.com/RemyLoveLogicAI/git-mcp/security/advisories

### Emergency Contact

For critical, time-sensitive security issues requiring immediate attention:
- **Email:** security@lovelogicai.com
- **Expected Response:** Within 4 hours during business hours

### Business Hours

- **Primary Support:** Monday - Friday, 9:00 AM - 5:00 PM PST
- **Emergency Support:** 24/7 for Critical severity issues

---

## 5. Security Update and Patch Process

### Regular Updates

- **Security Patches:** Released as soon as possible after verification
- **Dependency Updates:** Reviewed monthly for known vulnerabilities
- **Security Audits:** Conducted quarterly
- **Automated Scanning:** Continuous integration security checks

### Patch Release Process

1. **Vulnerability Confirmed:** Security team verifies the issue
2. **Patch Development:** Fix developed and tested in private branch
3. **Security Advisory:** Draft prepared (if public disclosure needed)
4. **Testing:** Comprehensive testing in staging environment
5. **Release:** Patch deployed to production
6. **Notification:** Users notified via GitHub releases and security advisory
7. **Documentation:** Update CHANGELOG and security documentation

### Notification Channels

Users will be notified of security updates through:

- **GitHub Security Advisories:** https://github.com/RemyLoveLogicAI/git-mcp/security/advisories
- **GitHub Releases:** https://github.com/RemyLoveLogicAI/git-mcp/releases
- **Email Notifications:** For registered users (if applicable)
- **Security Mailing List:** Subscribe at security@lovelogicai.com

### Emergency Patches

For critical vulnerabilities:
- Patches released within 24-48 hours
- Out-of-band security releases may be issued
- All users strongly urged to update immediately

---

## 6. Supported Versions Policy

### Currently Supported Versions

We provide security updates for the following versions:

| Version | Supported          | End of Support |
| ------- | ------------------ | -------------- |
| Latest (main) | :white_check_mark: | N/A |
| 2.x.x   | :white_check_mark: | TBD |
| 1.x.x   | :white_check_mark: | December 31, 2026 |
| < 1.0   | :x:                | No longer supported |

### Version Support Policy

- **Latest Stable Release:** Full security support
- **Previous Major Version:** Security updates for 12 months after new major release
- **Older Versions:** No security updates; users strongly encouraged to upgrade

### End-of-Life (EOL) Process

1. **6 Months Notice:** Announcement of upcoming EOL
2. **3 Months Notice:** Reminder and migration guide published
3. **EOL Date:** Security updates cease
4. **Post-EOL:** No further updates; critical issues may be addressed at discretion

### Upgrade Path

Users on unsupported versions should:
1. Review the CHANGELOG for breaking changes
2. Test upgrade in non-production environment
3. Follow migration guides (available in /docs/migration)
4. Contact support if assistance needed: security@lovelogicai.com

---

## Compliance and Certifications

This security policy supports compliance with:

- **SOC 2 Type II:** Trust Services Criteria
- **ISO/IEC 27001:** Information Security Management
- **PCI-DSS:** Payment Card Industry Data Security Standard
- **GDPR:** General Data Protection Regulation

### Security Controls

- Encryption at rest and in transit (TLS 1.3+)
- Regular vulnerability assessments
- Access controls and authentication mechanisms
- Audit logging and monitoring
- Incident response procedures
- Business continuity planning

---

## Additional Security Resources

### Best Practices for Users

- Keep your installation up to date
- Use strong, unique passwords
- Enable two-factor authentication where available
- Review access permissions regularly
- Monitor logs for suspicious activity
- Follow the principle of least privilege
- Validate Git repository sources before cloning
- Use secure MCP connections

### Security Documentation

- [Security Architecture](./docs/security/architecture.md)
- [Authentication Guide](./docs/security/authentication.md)
- [API Security](./docs/security/api-security.md)
- [Data Protection](./docs/security/data-protection.md)
- [MCP Protocol Security](./docs/security/mcp-security.md)

### Security Tools and Scanning

This repository uses:
- **Dependabot:** Automated dependency updates
- **CodeQL:** Static code analysis
- **Secret Scanning:** Prevent credential exposure
- **SAST/DAST:** Security testing in CI/CD pipeline

---

## Git-MCP Specific Security Considerations

### Git Operations Security

- All Git operations are executed in isolated environments
- Repository access is controlled via authentication tokens
- Git credentials are never stored in plain text
- Repository cloning is sandboxed to prevent arbitrary code execution

### MCP Protocol Security

- MCP connections use secure transport protocols
- All MCP messages are validated before processing
- Rate limiting prevents abuse of MCP endpoints
- Session tokens expire after inactivity

### Data Protection

- Sensitive data is encrypted both at rest and in transit
- User credentials are hashed using industry-standard algorithms
- API keys and tokens are rotated regularly
- Audit logs track all security-relevant events

---

## Questions or Concerns?

If you have questions about this security policy or need clarification:

- **Email:** security@lovelogicai.com
- **GitHub Discussions:** https://github.com/RemyLoveLogicAI/git-mcp/discussions
- **Documentation:** https://github.com/RemyLoveLogicAI/git-mcp/wiki

---

**Thank you for helping keep git-mcp and our users safe!**

---

*This security policy is subject to change. Please check back regularly for updates. This document was last reviewed on February 2, 2026.*
