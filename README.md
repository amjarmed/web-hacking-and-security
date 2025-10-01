# Roadmap to becoming competent at web hacking / bug bounty hunting

A bug bounty, penetration testing, or ethical hacking is a monetary reward given to white-hat hackers for successfully identifying and reporting security bugs and vulnerabilities in any software or application.

---

## 1. Foundational Knowledge (2-3 months)

### 1.1 Web Technologies

- HTML5: Document structure, forms, semantic elements
- CSS3: Selectors, box model, flexbox, grid
- JavaScript: DOM manipulation, events, AJAX, promises
- Modern frameworks overview (React, Angular, Vue)
- Backend basics (NodeJS, Python, Ruby, PHP)
- REST API concepts and testing

### 1.2 Networking Fundamentals

- TCP/IP stack and protocols
- HTTP/HTTPS request/response cycle
- DNS resolution and record types
- Cookies, sessions, and authentication
- Same-origin policy and CORS

### 1.3 Basic Tools

- Browser DevTools (Network, Console, Sources panels)
- Burp Suite Community Edition (Proxy, Repeater, Intruder)
- Command line basics and Linux fundamentals
- Git basics for version control

---

## 2. Security Fundamentals (3-4 months)

### 2.1 Core Web Vulnerabilities

- Cross-Site Scripting (XSS)
  - Reflected, Stored, and DOM-based XSS
  - Content Security Policy (CSP)
  - XSS prevention techniques
- SQL Injection
  - Union-based, Error-based, Blind
  - Database fingerprinting
  - WAF bypass techniques
- Server-Side Request Forgery (SSRF)
  - Cloud metadata endpoints
  - Internal service enumeration
  - Filter bypass techniques
- Insecure Direct Object References (IDOR)
  - Access control vulnerabilities
  - Parameter tampering
  - Mitigation strategies
- Broken Authentication
  - Session fixation
  - Weak password policies
  - Multi-factor authentication (MFA)
- Security Misconfiguration
  - Default credentials
  - Improperly configured headers
  - Hardening techniques
- Cross-Site Request Forgery (CSRF)
  - CSRF token implementation
  - SameSite cookie attributes
  - Double submit cookie pattern
- Broken Access Control
  - Privilege escalation
  - Horizontal and vertical privilege abuse
  - Access control design best practices
- Unvalidated Redirects and Forwards
  - Open redirect vulnerabilities
  - Phishing and redirection risks
  - Validation mechanisms
- Deserialization Vulnerabilities
  - Insecure deserialization risks
  - Object injection attacks
  - Secure deserialization techniques
- Sensitive Data Exposure
  - Unencrypted data in transit
  - Weak cryptographic storage
  - Secure communication protocols
- Insufficient Logging and Monitoring
  - Lack of audit logs
  - Undetected malicious activity
  - Monitoring best practices
- XML External Entity (XXE) Injection
  - XXE in XML parsers
  - Exploiting external entities
  - Secure XML processing
- HTTP Host Header Injection
  - Cache poisoning attacks
  - Open redirect abuse
  - Header validation mechanisms
- File Upload Vulnerabilities
  - Remote code execution via file uploads
  - Content type validation
  - Upload directory restrictions

### 2.2 Authentication & Authorization

- OAuth 2.0 and OpenID Connect
- JWT structure and common vulnerabilities
- Session management issues
- 2FA/MFA bypass techniques

### 2.3 Advanced Tools

- Burp Suite Professional features
- Custom wordlist creation
- Automated scanning tools
- Mobile testing tools (FRIDA, Objection)

### 2.4 Practice & Labs

- PortSwigger Web Security Academy
- OWASP Juice Shop
- Hackviser
- HackTheBox
- TryHackMe
- VulnHub

---

## 3. Advanced Techniques (4-6 months)

### 3.1 Advanced Vulnerabilities

- Race Conditions
  - Time-of-check to time-of-use
  - API race conditions
  - Payment system vulnerabilities
- Deserialization Vulnerabilities
  - Java deserialization
  - PHP object injection
  - NodeJS prototype pollution
- GraphQL Security
  - Introspection queries
  - Authorization flaws
  - DoS vectors

### 3.2 Cloud Security

- AWS security misconfigurations
- Azure service vulnerabilities
- GCP security issues
- Container security (Docker, Kubernetes)

### 3.3 Mobile Security

- Android app testing methodology
- iOS security assessment
- API security testing
- Mobile app bypass techniques

---

## 4. Professional Practice (Ongoing)

### 4.1 Bug Bounty Platforms

- HackerOne
  - Program selection strategies
  - Report writing best practices
  - Reputation building
- Bugcrowd
  - VRT understanding
  - Priority assessment
  - Program collaboration

### 4.2 Methodology Development

- Creating custom testing workflows
- Developing automation scripts
- Building recon infrastructure
- Documentation and note-taking systems

### 4.3 Community Engagement

- Contributing to open source tools
- Writing technical blog posts
- Speaking at security conferences
- Mentoring other researchers

---

## 5. Specialization Paths (Expert)

### 5.1 Web3 Security

- Smart contract auditing
- Blockchain vulnerabilities
- DeFi security
- Solidity security patterns

### 5.2 IoT Security

- Hardware hacking basics
- Firmware analysis
- RF communication security
- IoT protocols (MQTT, CoAP)

### 5.3 API Security

- REST API security testing
- GraphQL advanced exploitation
- gRPC security
- API versioning issues

---
