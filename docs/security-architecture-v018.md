# Enhanced Security Architecture v0.18

## Zero-Trust Data Plane
- Every scan: series integrity digest + Merkle-style lineage root (chained over OHLCV + strategy params + risk decision) + Parabolic SAR consistency check + source attestation.
- Residency: prefer declared region / sovereign cloud (e.g., SG); cross-border requires dual explicit attestation.
- Anomaly scoring: residual isolation-style proxy + directional/SAR inconsistency + volume profile divergence.

## Controls
- Paper-only: PermissionError on any live mode. No trader/withdrawal roles. Key separation.
- Expanded secret redaction (keys, seeds, tokens, PEM, base58, WIF, mnemonics, additional patterns).
- Hash-chained audit log with Merkle extension for lineage.
- PDPA tripwire, gitleaks CI, Ruff/Bandit-style lint (as in reference harness).
- Recommended: AES-256 at rest, TLS 1.3 in transit, external KMS/HSM, mutual TLS for research pipelines, continuous validation.

## Threats (additions)
| Threat | Control |
|---|---|
| Lineage tamper | Merkle root re-computed each scan |
| SAR proxy inconsistency | Explicit consistency check in zero-trust |
| Cross-border without dual att. | Residency preference + dual attestation note |

No live connectors. Research only. Not legal or compliance advice.
