# Security Policy

## Reporting Security Issues

If you discover a security vulnerability in APP, please report it privately before public disclosure.

Responsible disclosure helps protect users, operators, and ecosystem participants.

---

# Scope

Security reports may include:

- Authentication vulnerabilities
- Authorization bypasses
- Federation vulnerabilities
- Provenance tampering
- Signature verification issues
- Reputation manipulation
- Delegation escalation
- Denial of service vulnerabilities

---

# Responsible Disclosure Process

1. Report the issue privately.
2. Allow maintainers reasonable time to investigate.
3. Collaborate on remediation where appropriate.
4. Coordinate public disclosure once fixes are available.

---

# Cryptography

APP relies on modern cryptographic primitives including:

- SHA-256
- Ed25519
- Public Key Infrastructure concepts
- Signed provenance records

Implementations should avoid custom cryptography.

---

# Security Priorities

The highest priority security areas are:

1. Passport integrity
2. Provenance integrity
3. Federation trust
4. Ownership verification
5. Delegation controls
6. Reputation integrity

---

# Threat Model

APP assumes:

- Malicious agents may exist
- Federation participants may become compromised
- Credentials may be stolen
- Attestations may be abused
- Reputation systems may be targeted

The protocol is designed to make trust verifiable rather than assumed.

---

# Security Reviews

Security reviews and external audits are encouraged.

Contributors are encouraged to challenge assumptions and identify weaknesses.

---

# Security Mission

Trust infrastructure should be resilient, transparent, and verifiable.

Security is a foundational requirement of APP.
