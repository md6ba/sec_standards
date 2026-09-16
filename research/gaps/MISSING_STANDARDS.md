# Research Notes: Gaps

## 1. Missing Organizations

| Organization | Priority | Reason |
|---|---|---|
| ISO/IEC | HIGH | Foundational security standards (27001, 27002) |
| CIS | HIGH | Industry-standard security controls |
| OpenSSF | MEDIUM | Supply chain security best practices |
| NSA/CNSA | MEDIUM | PQC migration mandate (CNSA 2.0) |
| PCI SSC | MEDIUM | Payment card security |
| IEC | LOW | Industrial control system security |
| BSI (Germany) | LOW | National security guidelines |
| ANSSI (France) | LOW | National security guidelines |
| NCSC-UK | LOW | National security guidelines |

## 2. Missing Document Types

- **ETSI PQC migration strategy TR 103 619** — known but not downloaded
- **NCCoE practice guides** — not investigated
- **NIST SP 800-175A** (commercial PKI guidance) — not collected

## 3. Potential ISO Accessibility

Some ISO standards may be accessible via:
- National standards bodies (e.g., BSI, DIN) with preview
- IETF references to ISO standards
- University library access

## 4. Datasets Not Yet Collected

- **CPE dictionary** — partially collected, full dictionary is large
- **CAPEC** (Common Attack Pattern Enumeration) — attack patterns database
- **ATT&CK** (Adversarial Tactics, Techniques, Common Knowledge) — MITRE ATT&CK
- **OWASP CAPEC** references
- **NIST SP 800-53 controls** machine-readable format (OSCAL)

## 5. Experimental/Mislabeled PQC

**Verified STANDARDIZED:**
- ML-KEM (FIPS 203) — Aug 2024
- ML-DSA (FIPS 204) — Aug 2024
- SLH-DSA (FIPS 205) — Aug 2024

**Verified DRAFT (not yet standardized):**
- FN-DSA (FIPS 206) — former FALCON, draft expected 2025-2026
- HQC — Round 4 alternate, draft expected ~2027

**Known EXPERIMENTAL:**
- BIKE — Round 4 alternate, not selected for standardization
- Classic McEliece — Round 4 alternate, NIST IR in progress

The collection correctly labels all three categories.

---

*Last updated: 2026-09-16*
