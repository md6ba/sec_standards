# sec_standards — Security Standards Knowledge Base

A locally stored, versioned, traceable collection of authoritative security
standards, frameworks, guidelines, protocols, and cryptographic standards.

**Purpose:** Reference material for building security-sensitive software,
conducting security assessments, implementing cryptographic systems, and
maintaining compliance with recognized standards.

> **This is a reference collection — not an implementation guide.**
> The next phase transforms this knowledge base into machine-readable
> security rules and an agent system prompt.

---

## 📊 Collection Overview

| Metric | Value |
|--------|-------|
| **Total files** | 154 |
| **Total size** | 96 MB |
| **Organizations** | 10 |
| **Documents cataloged** | 146 |
| **Cross-references** | 8 groups |
| **SHA-256 verified** | All files |

---

## 🏛️ Organizations Covered

| Organization | Type | Documents |
|---|---|---|
| **NIST** | US Federal | 34 |
| **IETF** | International Standards | 78 |
| **NVD** | Vulnerability Database | 9 |
| **OWASP** | Open Source Security | 6 |
| **CISA** | US Government | 3 |
| **ETSI** | European Standards | 2 |
| **FIRST** | Incident Response | 2 |
| **MITRE (CWE)** | Research | 2 |
| **CFRG (IRTF)** | Crypto Research | 1 |
| **SLSA** | Supply Chain | 1 |

---

## 🔐 Cryptographic Coverage

### Classical Cryptography
- **Symmetric Encryption:** AES (FIPS 197), modes (SP 800-38A/B/D/F)
- **Hash Functions:** SHA-2 (FIPS 180-4), SHA-3 (FIPS 202)
- **MAC:** HMAC (FIPS 198-1), CMAC (RFC 4493), GMAC
- **Key Derivation:** HKDF (RFC 5869), PBKDF2 (RFC 8018), scrypt (RFC 7914), Argon2 (RFC 9106)
- **AEAD:** GCM (SP 800-38D), CCM (RFC 4309), ChaCha20-Poly1305 (RFC 8439)
- **Key Wrap:** RFC 3394, SP 800-38F
- **Public-Key:** RSA, ECDSA (RFC 5480), EdDSA (RFC 8032)
- **Key Exchange:** DH (RFC 2631), ECDH (RFC 4492), X25519/X448 (RFC 7748), DHE (RFC 3526)
- **DRBG:** SP 800-90A (deterministic), 90B (entropy), 90C (construction)
- **Key Management:** SP 800-57 Part 1 (key lifecycle)

### Post-Quantum Cryptography (PQC)

**Standardized (9):**
- FIPS 203 (ML-KEM) — Module-Lattice KEM
- FIPS 204 (ML-DSA) — Module-Lattice Digital Signature
- FIPS 205 (SLH-DSA) — Stateless Hash-Based Signature
- NIST SP 800-208 (Stateful HBS)
- RFC 8554 (LMS), RFC 8391 (XMSS) — Stateful hash-based
- RFC 8784 (PQ-PPK for IKEv2)
- RFC 9370 (Multiple Key Exchanges in IKEv2)
- RFC 9954 (Hybrid Key Exchange in TLS 1.3)

**Draft (7):**
- NIST IR 8547 (PQC Transition)
- NIST IR 8545 (4th Round Status)
- draft-ietf-tls-ecdhe-mlkem, draft-ietf-tls-mlkem
- draft-ietf-uta-pqc-app, draft-irtf-cfrg-hybrid-kems
- draft-pquip-pqc-migration

**Research/Informational (2):**
- ETSI TR 103 616 (Quantum-Safe Signatures)
- ETSI TR 103 949 (QSC Algorithm Profiles)

**Experimental / Not Yet Standardized:**
- FN-DSA (FIPS 206) — draft (former FALCON)
- HQC — Round 4 alternate, FIPS expected ~2027

---

## 🌐 Network & Protocol Security

| Protocol | RFCs |
|----------|------|
| TLS 1.3 | RFC 8446 + security RFCs (7366, 7465, 7568, 7627) |
| TLS 1.2 | RFC 5246 |
| SSH | RFC 4251, 4252, 4253, 4254, 4419 |
| IPsec/IKEv2 | RFC 4301, 4302, 4303, 7296 |
| DNSSEC | RFC 4033, 4034, 4035 |
| HTTP/2 | RFC 7540 |
| HTTP | RFC 9110, 9111, 7230 |
| Certificate Transparency | RFC 6962 |
| PKI/X.509 | RFC 5280, 5758 |

---

## 🔑 Identity & Authentication

| Standard | Document |
|----------|----------|
| OAuth 2.0 | RFC 6749 |
| OAuth 2.0 Threat Model | RFC 6819 |
| PKCE | RFC 7636 |
| Token Introspection | RFC 7662 |
| Token Revocation | RFC 7009 |
| JWT | RFC 7519 |
| JWS | RFC 7515 |
| JWE | RFC 7516 |
| JWA | RFC 7518 |
| OAuth 2.0 for Native Apps | RFC 8252 |
| OAuth 2.0 for Browser Apps | RFC 8210 |
| JWT Access Tokens | RFC 9068 |
| ACME | RFC 8555 |
| OpenID Connect | openid-connect-core-1_0.html |
| WebAuthn Level 2 | webauthn-2.html |
| FIDO2 / CTAP2 | fido-ctap2.html |
| NIST Digital Identity | SP 800-63A, 63B, 63-4 |

---

## 🐛 Vulnerability Management

| Resource | Description |
|----------|-------------|
| CVE | NVD JSON exports (2023-2026, modified, recent) |
| CWE | MITRE taxonomy (1000.csv, full) |
| CVSS v3.1 | Vector schema |
| CVSS v4.0 | Vector schema |
| CPE | Common Platform Enumeration |

---

## 🏗️ Secure Software Development

| Topic | Document |
|-------|----------|
| SSDF | NIST SP 800-218 (Secure Software Development Framework) |
| Secure by Design | CISA 2023 |
| Supply Chain Risk | NIST SP 800-161 |
| Software Acquisition | CISA SAG |
| SLSA | Supply-chain Levels for Software Artifacts |
| Secure Coding | OWASP Secure Coding Practices |

---

## 📁 Project Structure

```
sec_standards/
├── README.md                    ← You are here
├── CATALOG.yaml                 ← Authoritative catalog (146 entries)
├── SOURCES.yaml                 ← Source organizations & access status
├── COLLECTION_STATUS.md         ← Discovery progress
├── VERSION_HISTORY.md           ← Version tracking
├── LICENSES.md                  ← Legal access classifications
├── COLLECTION_REPORT.md         ← Coverage statistics
│
├── standards/                   ← Full documents by organization
│   ├── nist/                    ← 34 NIST publications
│   ├── ietf/                    ← 78 RFCs (TLS, SSH, IPsec, PKI, HTTP, OAuth)
│   ├── owasp/                   ← 6 OWASP guidelines
│   ├── cisa/                    ← 3 CISA guidance documents
│   ├── fips/                    ← FIPS 140-3, 180-4, 186-5
│   ├── other/                   ← WebAuthn, OpenID Connect, FIDO2
│   └── slsa/                    ← SLSA specification
│
├── cryptography/                ← Domain-specific crypto standards
│   ├── classical/               ← AES, SHA, HMAC, HKDF, X25519, Argon2...
│   │   ├── nist/                ← 14 NIST crypto pubs
│   │   └── ietf/                ← 21 IETF RFCs
│   ├── pqc/                     ← Post-quantum cryptography
│   │   ├── nist/                ← FIPS 203/204/205, IRs
│   │   ├── ietf/                ← 10 PQC RFCs/drafts
│   │   ├── etsi/                ← 2 ETSI TRs
│   │   └── cfrg/                ← CFRG draft
│   ├── key-management/          ← SP 800-57
│   └── randomness/              ← SP 800-90A/B/C
│
├── datasets/                    ← Machine-readable security data
│   ├── cve/                     ← NVD JSON exports
│   ├── cwe/                     ← MITRE CWE taxonomy
│   ├── cvss/                    ← CVSS v3.1, v4.0 vectors
│
├── skills/                      ← AI Agent Skills
│   └── security-standards/      ← Hermes Skill (MAP to this KB)
│       └── SKILL.md             ← Domain map, gates, retrieval procedure
│
└── research/
    └── gaps/                    ← Missing standards & next actions
```

---

## 🧭 Security Domain Map

```
SECURITY
├── Governance/Risk (NIST CSF, RMF, ISO 27000)
├── Secure Software Dev (SSDF, OWASP, SLSA, OpenSSF)
├── Cryptography (AES, SHA, HMAC, AEAD, PQC, DRBG)
├── Post-Quantum (ML-KEM, ML-DSA, SLH-DSA, hybrid, migration)
├── Network Security (TLS, IPsec, SSH, DNSSEC, PKI, HTTP)
├── Identity & Auth (OAuth, OIDC, WebAuthn, FIDO2, MFA)
├── Application Security (OWASP ASVS, API security, sessions)
├── Vulnerability Management (CVE, CWE, CVSS, CPE)
├── Supply Chain (SBOM, SLSA, provenance, artifact integrity)
├── Security Testing (SAST, DAST, fuzzing, pen testing)
└── Threat Modeling (attack surface, trust boundaries, abuse cases)
```

---

## 🔍 Using This Knowledge Base

### 1. Search by Domain

```bash
# Find all cryptography standards
grep -A 20 "cryptography:" CATALOG.yaml

# Find PQC documents
grep -i "pqc\|post.quantum\|ml.kem\|ml.dsa\|slh" CATALOG.yaml

# Find TLS RFCs
grep -i "tls" CATALOG.yaml
```

### 2. Search by Organization

```bash
# All NIST publications
grep -A 30 "nist/" CATALOG.yaml

# All IETF RFCs
grep -A 30 "ietf/" CATALOG.yaml
```

### 3. Search by Tag

```bash
# High-relevance standards
grep "relevance:" CATALOG.yaml | head -20
```

### 4. Verify Document Integrity

```bash
# Check SHA-256 for any document
sha256sum standards/nist/NIST.SP.800-218.pdf
# Compare with CATALOG.yaml entry
```

---

## ⚖️ Authority Hierarchy

When sources follow this priority (higher overrides lower):

1. **Law / regulatory requirement** (highest authority)
2. **Official standard** (NIST FIPS, ISO, IETF RFC)
3. **Official technical guidance** (NIST SP, CISA)
4. **Protocol specification** (IETF RFC)
5. **Established framework** (OWASP, NIST CSF)
6. **Project security policy**
7. **General best practice**
8. **Agent preference** (lowest authority)

**When sources conflict:** Retrieve both, identify versions, determine applicability, report the conflict — never invent a resolution.

---

## 🚧 Gaps & Next Actions

### Critical Gaps (Not Yet Collected)
- **ISO/IEC 27000 family** — Copyrighted, metadata-only
- **CIS Controls v8** — Requires email registration
- **OpenSSF Best Practices** — Not yet collected
- **NSA/CNSA 2.0** — PQC migration mandate, URL known but not downloaded

### Coverage Gaps
- **ETSI PQC migration strategy TR 103 619** — Known but not downloaded
- **NIST NCCoE practice guides** — Not investigated
- **PCI DSS** — Payment industry security standard
- **IEC 62443** — Industrial control system security
- **BSI/ANSSI/NCSC-UK** — National security guidelines
- **CAPEC** — Common Attack Pattern Enumeration
- **MITRE ATT&CK** — Adversarial tactics framework

### How to Contribute

1. **Add a new standard:**
   - Place document in appropriate subdirectory
   - Add entry to `CATALOG.yaml`
   - Update `SOURCES.yaml` and `COLLECTION_STATUS.md`

2. **Update an existing standard:**
   - Do NOT overwrite the old version
   - Create new version: `document-v1.pdf` → `document-v2.pdf`
   - Update `VERSION_HISTORY.md`
   - Update `CATALOG.yaml` with new entry

3. **Report a gap:**
   - Add to `research/gaps/MISSING_STANDARDS.md`
   - Include source URL if known

---

## 📜 Legal Status Classifications

| Code | Meaning |
|------|---------|
| `official_public` | Official document, publicly available |
| `official_restricted` | Official document, access restricted |
| `metadata_only` | Not freely available; metadata recorded |
| `draft` | Published draft, not finalized |
| `experimental` | Experimental, not for production |
| `deprecated` | Superseded or withdrawn |

---

## 🤖 Security Standards Skill (Hermes AI Agent)

This knowledge base includes a companion **Hermes Skill** that teaches AI agents
how to use it as an authoritative source for security-sensitive work.

### What the Skill Does

- **Maps** every security question to the correct domain and standards
- **Forces** mandatory Security Change Gate, Cryptography Gate, and PQC Gate
- **Enforces** authority hierarchy (law > standard > guidance > framework > policy)
- **Requires** evidence-based answers (WHAT, WHY, SOURCE, VERSION, WHERE)
- **Prevents** relying on model memory — always retrieves from `sec_standards`

### Installing the Skill

The skill is included in this repository at `skills/security-standards/SKILL.md`.
To install it in your Hermes Agent:

```bash
# Clone this repo (if not already)
git clone https://github.com/md6ba/sec_standards.git

# Copy skill to your Hermes skills directory
cp -r sec_standards/skills/security-standards ~/.hermes/profiles/domino/skills/security/

# Or use Hermes skill management:
# 1. Open Hermes
# 2. Run: /install-plugin security-standards
# 3. Or manually place SKILL.md in skills/security/security-standards/
```

### Skill Architecture

```
SECURITY STANDARDS SKILL (the MAP)
            │
            │ "KNOW WHERE TO LOOK"
            ▼
      sec_standards/ (the KNOWLEDGE BASE)
            │
            │ "FIND THE SOURCE"
            ▼
   Relevant Requirement
            │
            │ "APPLY IT WITH EVIDENCE"
            ▼
     Project Security
```

### Validation (5 Scenarios)

| Scenario | Behavior |
|----------|----------|
| "Add encrypted transport" | Identifies Network Security + Crypto, retrieves TLS standards |
| "Choose a cryptographic algorithm" | Consults FIPS, verifies status, provides evidence |
| "Make this post-quantum secure" | Activates PQC gate, distinguishes standardized vs experimental |
| "Fix a security bug" | Determines affected properties, inspects standards, tests |
| "Use the fastest algorithm" | Security constraints override performance |

### Key Principle

> **The Skill is the MAP, this knowledge base is the SOURCE OF TRUTH.**
> Never duplicate actual standards into the agent's procedural memory.

---

## 📈 Statistics

### Document Type Distribution

| Type | Count |
|------|-------|
| RFC (text) | 79 |
| Standard (PDF) | 49 |
| Dataset | 9 |
| Document | 6 |
| Specification (HTML) | 3 |

### Status Distribution

| Status | Count |
|--------|-------|
| Standardized | 90 |
| Informational | 30 |
| Document | 8 |
| Recommendation | 6 |
| Standard | 5 |
| Guideline | 3 |
| Best Current Practice | 2 |
| Experimental | 1 |
| Framework | 1 |

---

## 📅 Version History

- **v1.0** (2026-09-16): Initial collection pass — 146 entries, 10 organizations, 154 files

---

## 📄 License

This project collects metadata and references to security standards. Individual
documents retain their original copyright and licensing:

- **US Government publications** (NIST, CISA): Public domain
- **IETF RFCs**: Publicly available
- **OWASP**: CC-BY-SA 4.0
- **SLSA**: Apache 2.0
- **ISO/IEC**: Copyrighted — metadata-only references
- **ETSI**: Mixed — some freely available, some restricted

---

## 🔗 Related Projects

- **security-standards Hermes Skill** — Teaches agents how to use this KB
- **QFort** — Post-quantum secure tunnel (uses these standards as reference)
- **sec_standards/collections** — Machine-readable security datasets

---

*Collection started: 2026-09-16*
*Last updated: 2026-09-16*
*Maintained by: [Your Name]*
