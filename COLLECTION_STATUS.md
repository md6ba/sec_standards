# Collection Status

## Discovery Pass

### NIST (National Institute of Standards and Technology)
- [x] Cybersecurity Framework (CSF) v2.0
- [x] SP 800 series: 53, 63A, 63B, 131A, 161, 175B, 207, 218
- [x] FIPS: 140-3, 180-4, 186-5
- [x] PQC: FIPS 203, 204, 205; IR 8545, 8547; SP 800-208
- [x] Key Management: SP 800-57
- [x] Randomness: SP 800-90A, 90B, 90C
- [x] Supply Chain: SP 800-161
- [x] Zero Trust: SP 800-207
- [x] Identity: SP 800-63A, 800-63B
- [x] Risk Management: SP 800-30, 800-37
- [x] Cryptographic Modes: SP 800-38A/B/D/F

### IETF
- [x] TLS: RFC 8446, 5246, 7366, 7465, 7568, 7627
- [x] SSH: RFC 4251, 4252, 4253, 4254, 4419
- [x] IPsec: RFC 4301, 4302, 4303, 7296
- [x] DNSSEC: RFC 4033, 4034, 4035
- [x] HTTP Security: RFC 7230, 7540, 7838, 8811, 9110, 9111
- [x] PKI: RFC 5280, 5758, 6962
- [x] Crypto Algorithms: RFC 2631, 3279, 3394, 3526, 3686, 3766, 4309, 4492, 4493, 4868, 5084, 5114, 5116, 5480, 5647, 5649, 5903, 5915, 6979, 7748, 7914, 8018, 8032, 8439, 9106
- [x] OAuth/JWT: RFC 6749, 6819, 7009, 7515, 7516, 7518, 7519, 7636, 7662, 8252, 8555, 9068
- [x] PQC: RFC 8391, 8554, 8784, 9370, 9954; drafts for TLS, SSH, UTA, migration

### OWASP
- [x] Top 10 (2021)
- [x] Top 10 (2025)
- [x] ASVS v5.0.0
- [x] SAMM v2
- [x] API Security Top 10 (2023)
- [x] Secure Coding Practices

### CISA
- [x] Secure by Design
- [x] Software Acquisition Guide
- [x] ICT SCRM Fact Sheet

### NVD / CVE / CWE / CVSS
- [x] CVE datasets (2023, 2024, 2025, modified, recent, pages)
- [x] CWE 1000.csv, full taxonomy
- [x] CVSS v3.1, v4.0 vectors

### Post-Quantum Cryptography
- [x] ML-KEM (FIPS 203) — standardized
- [x] ML-DSA (FIPS 204) — standardized
- [x] SLH-DSA (FIPS 205) — standardized
- [x] Transition guidance (NIST IR 8547)
- [x] Hybrid approaches (RFC 9954, multiple drafts)
- [x] Stateful hash-based signatures (LMS/XMSS)

### Other
- [x] WebAuthn Level 2
- [x] OpenID Connect Core 1.0
- [x] FIDO2 / CTAP2

---

## Summary

| Organization | Documents | Status |
|---|---|---|
| NIST | 34 | Downloaded |
| IETF | 78 | Downloaded |
| NVD | 9 | Downloaded (datasets) |
| OWASP | 6 | Downloaded |
| CISA | 3 | Downloaded |
| ETSI | 2 | Downloaded |
| FIRST | 2 | Downloaded (datasets) |
| MITRE (CWE) | 2 | Downloaded (datasets) |
| CFRG | 1 | Downloaded |
| SLSA | 1 | Downloaded |
| **Total** | **138** | |

---

## Gaps and Next Actions

### ISO/IEC (metadata-only)
- ISO/IEC 27000 family, 27001, 27002, 27017, 27018, 27701, 15408, 23894
- Status: Copyrighted — metadata only

### CIS
- CIS Controls v8, CIS Benchmarks
- Status: Requires registration for benchmarks

### OpenSSF
- Best practices, scorecard documentation
- Status: Not yet collected

### Not Yet Investigated
- NSA/CNSA 2.0 mandate
- NIST NCCoE practice guides
- BSI (Germany), ANSSI (France), NCSC-UK
- PCI DSS
- IEC 62443 (industrial security)

### PQC Coverage
**Standardized (9):** FIPS 203/204/205, SP 800-208, RFC 8554/8391/8784/9370/9954
**Draft (7):** NIST IR 8547/8545, drafts for TLS/SSH/UTA/migration
**Research (2):** ETSI TR 103 616/949

---

*Last updated: 2026-09-16*
