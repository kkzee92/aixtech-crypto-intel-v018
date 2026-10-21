# AIxTech Crypto Intel v0.18: Enhanced Paper-Only Trading Information System

Research harness for automated cryptocurrency **information** systems and paper strategy evaluation. Strictly paper-only: no live orders, no exchange secrets, not financial advice.

Builds on previous versions (including kkzee92/aixtech-crypto-intel, v0.17 Supertrend/volume delta, and the style of [zeekiankok92/aixtech-agent-harness-demo](https://github.com/zeekiankok92/aixtech-agent-harness-demo) for CI gates, PDPA tripwire, AI disclosure, and human review).

## v0.18 Enhancements

- Parabolic SAR-style acceleration factor proxy for trailing trend confirmation on Major, RWA, and L2 strategies.
- Refined volume profile / delta imbalance with multi-window acceleration for Large-cap alt and Meme filters.
- Multi-asset correlation regime detection with dynamic threshold for portfolio-level risk gates.
- Advanced data lineage: Merkle-style chained digests over series + strategy params + risk decisions.
- Enhanced anomaly scoring: residual isolation-style + Parabolic SAR inconsistency + volume profile divergence.
- Expanded zero-trust: continuous re-validation including SAR consistency and lineage root.
- Data residency + sovereign cloud notes; cross-border requires dual attestation.

## Asset Class Strategies (Enhanced)

| Class | Key Enhancements | Risk Cap |
|-------|------------------|----------|
| Major | Parabolic SAR alignment + Supertrend + multi-factor | 8% |
| Large-cap alt | Volume profile delta + multi-window accel | 4% |
| Stablecoin | Unchanged depeg alerts | 0% |
| DeFi | Supertrend + volume in calm regimes | 2% |
| Meme | Burst + volume profile accel | 0.5% |
| L2 | Relative SAR excess vs benchmark | 3% |
| RWA | Slow SAR + gap halt | 2% |
| Perpetual | Volume delta + funding consistency | 2% |

Full details in docs/.

## Security Architecture

- Zero-trust re-validation on every scan: integrity + Merkle lineage root + SAR consistency + source attestation.
- Data residency preferred (e.g., SG / sovereign); cross-border dual attestation required.
- Hash-chained audit with Merkle extension, expanded secret redaction, PDPA tripwire.
- Paper-only PermissionError guards. Recommended AES-256, TLS 1.3, external KMS, mTLS.

## Run (synthetic only)

See prior versions for CLI patterns (scan, brief, posture, demo on fixtures/candles_synthetic.json). All on synthetic fixtures only.

**Disclaimer**: Research only. Not investment advice. No live trading. Scores describe the synthetic fixture, not future returns.
