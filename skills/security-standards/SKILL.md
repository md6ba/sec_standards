---
name: security-standards
description: "Use sec_standards for crypto, protocols, compliance work."
version: 1.0.0
last_updated: 2026-09-16
author: MDBA (md6ba), Hermes Agent
license: MIT
platforms: [linux, macos, windows]
metadata:
  hermes:
    tags: [security, standards, map, reference, cryptography, protocols, compliance]
    related_skills: [security-scientist, security-negative-testing, requesting-code-review]
---

# Security Standards Skill

MAP to sec_standards. Authority hierarchy, retrieval, and gates for security-sensitive work.

## Architecture

```
SECURITY STANDARDS SKILL (this file)
            │ "KNOW WHERE TO LOOK"
            ▼
      sec_standards (knowledge base)
            │ "FIND THE SOURCE"
            ▼
   Relevant Requirement → APPLY IT → Project Security
```

## When to Use

- Security-sensitive code changes (auth, crypto, transport, secrets)
- Choosing cryptographic algorithms or parameters
- Designing secure protocols or sessions
- Implementing key management or randomness
- Evaluating post-quantum requirements
- Security testing or audit preparation
- Any task where an authoritative standard applies

**Don't use for:** Non-security tasks (UI, business logic, performance)

## Knowledge Base

```
sec_standards/
├── CATALOG.yaml          ← authoritative catalog
├── SOURCES.yaml          ← source organizations
├── COLLECTION_STATUS.md  ← progress
├── VERSION_HISTORY.md    ← version tracking
├── LICENSES.md           ← legal access
├── COLLECTION_REPORT.md  ← coverage stats
├── standards/            ← full documents
│   ├── nist/ ietf/ owasp/ cisa/ fips/ other/
├── cryptography/         ← classical, PQC, key-mgmt, randomness
├── protocols/            ← TLS, SSH, IPsec, PKI, HTTP
├── datasets/             ← CVE, CWE, CVSS
└── research/             ← gaps, conflicts, deprecated
```

## Domain Map

```
SECURITY
├── Governance/Risk (NIST CSF, RMF)
├── Secure Dev (SSDF, OWASP, SLSA)
├── Cryptography (AES, SHA, HMAC, AEAD, PQC)
├── PQC (ML-KEM, ML-DSA, SLH-DSA)
├── Network (TLS, IPsec, SSH, DNSSEC, PKI)
├── Identity (OAuth, OIDC, WebAuthn)
├── Appsec (ASVS, API security)
├── Vuln Mgmt (CVE, CWE, CVSS)
├── Supply Chain (SBOM, SLSA)
├── Testing (SAST, DAST, fuzzing)
└── Threat Modeling
```

## Authority Hierarchy

1. Law/regulatory (highest)
2. Official standard (FIPS, ISO, RFC)
3. Technical guidance (NIST SP, CISA)
4. Protocol spec (IETF RFC)
5. Framework (OWASP, NIST CSF)
6. Project policy
7. Best practice
8. Agent preference (lowest)

**Conflicts:** Retrieve both, identify versions, report, never invent resolution.

## Retrieval Procedure

1. **Classify** the task to domain(s)
2. **Search** CATALOG.yaml: `grep -i <domain> CATALOG.yaml`
3. **Read** the actual document from local_path
4. **Verify** status: standardized | draft | informational | experimental | deprecated
5. **Apply** with citation (document ID, version, section)

## Security Change Gate

```
[ ] Identify affected security properties
[ ] Identify applicable standards
[ ] Retrieve requirements from sec_standards
[ ] Check crypto/protocol implications
[ ] Check downgrade/replay/nonce/key risks
[ ] Implement → Test → Review → Re-check
```

## Cryptography Gate

```
[ ] Algorithm selection (sec_standards/cryptography/)
[ ] Security strength, key size, nonce/IV
[ ] Key lifecycle, rotation, derivation
[ ] Authentication, integrity, replay protection
[ ] Forward secrecy, algorithm agility
[ ] Deprecation status, quantum resistance
```

## PQC Gate

```
[ ] NIST PQC status (standardized vs draft vs experimental)
[ ] ML-KEM, ML-DSA, SLH-DSA (standardized)
[ ] Hybrid classical/PQC requirements
[ ] Migration (NIST IR 8547)
[ ] Harvest-now-decrypt-later risk
```

## Evidence Requirements

Answer: WHAT, WHY, SOURCE, VERSION, WHERE, IMPLEMENTATION, VERIFICATION.

**Never copy full standards.** Use concise evidence references.

## Failure Handling

1. Search sec_standards more broadly
2. Check cross-references and related domains
3. Report gap clearly
4. **Never fabricate a standard**

## No Duplication Rule

**This Skill is the MAP, not the knowledge.**

Ask: "Does Hermes need this as a permanent rule, or can it retrieve from sec_standards?"

If retrieval suffices, keep it out of this Skill.

## Related Skills

- `security-scientist` — security analysis, threat modeling
- `security-negative-testing` — paired negative tests
- `requesting-code-review` — pre-commit security scan
- `systematic-debugging` — security bug investigation
- `test-driven-development` — security tests
