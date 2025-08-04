---
mode: agent
description: Comprehensive security audit to identify vulnerabilities and suggest security improvements
---

Your task is to perform a comprehensive security audit of the selected code, identifying potential vulnerabilities, security weaknesses, and providing actionable recommendations for improvement.

## Security Audit Scope

### Code Security Analysis
- **Input Validation**: Check for proper sanitization and validation of user inputs
- **Authentication & Authorization**: Review access controls and permission checks
- **Data Protection**: Analyze handling of sensitive data and secrets
- **Injection Vulnerabilities**: Look for SQL, NoSQL, command, and script injection risks
- **Cryptographic Implementation**: Review encryption, hashing, and key management

### Application Security
- **Session Management**: Check session handling, timeouts, and storage
- **Error Handling**: Ensure errors don't leak sensitive information
- **Logging & Monitoring**: Review what's logged and how it's protected
- **Configuration Security**: Check for secure configuration practices
- **Dependency Security**: Analyze third-party library vulnerabilities

## Security Audit Output Format

```markdown
## Security Audit Report

### Executive Summary
**Overall Risk Level**: [Critical/High/Medium/Low]
**Critical Issues Found**: [Number]
**Recommendations Priority**: [List top 3 priority items]

### Vulnerability Assessment

#### Critical Vulnerabilities
1. **[Vulnerability Type]**
   - **Location**: [File:Line or function name]
   - **Risk Level**: Critical
   - **Description**: [Detailed description of the vulnerability]
   - **Potential Impact**: [What could happen if exploited]
   - **Exploit Scenario**: [How an attacker might exploit this]
   
   **Vulnerable Code**:
   ```code
   [Show the problematic code]
   ```
   
   **Recommended Fix**:
   ```code
   [Show the secure implementation]
   ```
   
   **Additional Measures**: [Extra security steps to consider]

#### High/Medium/Low Vulnerabilities
[Repeat the same format for other severity levels]

### Security Best Practices Review

#### Input Validation & Sanitization
- **Current State**: [Assessment of current input handling]
- **Gaps Identified**: [Missing validation or sanitization]
- **Recommendations**: [Specific improvements needed]

#### Authentication & Authorization
- **Current State**: [Assessment of auth implementation]
- **Gaps Identified**: [Weak points in access control]
- **Recommendations**: [Security improvements needed]

#### Data Protection
- **Sensitive Data Handling**: [How sensitive data is processed]
- **Encryption Status**: [What's encrypted and what's not]
- **Recommendations**: [Data protection improvements]

### Security Checklist Results

#### OWASP Top 10 Analysis
- [ ] **A01: Broken Access Control** - [Status/Findings]
- [ ] **A02: Cryptographic Failures** - [Status/Findings]
- [ ] **A03: Injection** - [Status/Findings]
- [ ] **A04: Insecure Design** - [Status/Findings]
- [ ] **A05: Security Misconfiguration** - [Status/Findings]
- [ ] **A06: Vulnerable Components** - [Status/Findings]
- [ ] **A07: Authentication Failures** - [Status/Findings]
- [ ] **A08: Software Integrity Failures** - [Status/Findings]
- [ ] **A09: Logging Failures** - [Status/Findings]
- [ ] **A10: Server-Side Request Forgery** - [Status/Findings]

### Implementation Roadmap
1. **Immediate Actions** (Fix within 24-48 hours)
2. **Short-term Improvements** (Complete within 1-2 weeks)
3. **Long-term Enhancements** (Plan for next development cycle)

### Monitoring & Prevention
- **Security Monitoring**: [What to monitor for ongoing security]
- **Automated Testing**: [Security tests to add to CI/CD]
- **Regular Audits**: [Recommended audit frequency and scope]
```

## Common Security Vulnerabilities to Check

### Input/Output Security
- **SQL Injection**: Parameterized queries, input sanitization
- **Cross-Site Scripting (XSS)**: Output encoding, Content Security Policy
- **Command Injection**: Input validation, avoid system calls with user input
- **Path Traversal**: Validate file paths, restrict file access
- **LDAP Injection**: Proper LDAP query construction

### Authentication & Session Management
- **Weak Password Policies**: Password complexity, storage (hashing)
- **Session Fixation**: Proper session regeneration
- **Insufficient Session Expiration**: Timeout configurations
- **Insecure Session Storage**: Secure cookies, session data protection
- **Broken Authentication**: Multi-factor authentication, account lockout

### Authorization & Access Control
- **Privilege Escalation**: Proper role-based access control
- **Insecure Direct Object References**: Authorization checks for resources
- **Missing Authorization**: Protected endpoints and operations
- **Broken Access Control**: Proper permission validation

### Data Protection
- **Sensitive Data Exposure**: Encryption at rest and in transit
- **Insufficient Cryptography**: Strong encryption algorithms and key management
- **Insecure Storage**: Secure configuration of databases and file systems
- **Data Leakage**: Information disclosure in errors and logs

### Configuration & Deployment
- **Security Misconfiguration**: Default credentials, unnecessary services
- **Insecure Communications**: HTTPS/TLS configuration
- **Vulnerable Dependencies**: Outdated libraries and frameworks
- **Insufficient Logging**: Security event monitoring and alerting

## Language-Specific Security Considerations

### Web Applications
- **CORS Configuration**: Cross-origin resource sharing policies
- **Content Security Policy**: XSS protection headers
- **HTTP Security Headers**: HSTS, X-Frame-Options, etc.
- **Cookie Security**: Secure, HttpOnly, SameSite attributes

### API Security
- **Rate Limiting**: Prevent abuse and DoS attacks
- **Input Validation**: Schema validation for JSON/XML
- **Authentication Tokens**: JWT security, token expiration
- **API Versioning**: Secure handling of different API versions

### Database Security
- **Connection Security**: Encrypted connections, connection pooling
- **Query Security**: Parameterized queries, stored procedures
- **Access Control**: Database user permissions, principle of least privilege
- **Data Encryption**: Field-level encryption for sensitive data

### Mobile/Client-Side Security
- **Local Storage**: Secure storage of sensitive data
- **Network Communication**: Certificate pinning, request encryption
- **Code Obfuscation**: Protection against reverse engineering
- **Runtime Protection**: Anti-tampering measures

## Security Testing Recommendations

### Automated Security Testing
- **SAST (Static Analysis)**: Tools like SonarQube, Checkmarx
- **DAST (Dynamic Analysis)**: Tools like OWASP ZAP, Burp Suite
- **Dependency Scanning**: Tools like Snyk, WhiteSource
- **Container Security**: Docker image scanning

### Manual Security Testing
- **Penetration Testing**: Professional security assessment
- **Code Review**: Security-focused peer review
- **Threat Modeling**: Systematic threat analysis
- **Security Architecture Review**: Design-level security assessment
