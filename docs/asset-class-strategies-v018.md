# Enhanced Asset-Class Strategies v0.18

Research heuristics only. Not predictive. Builds on v0.17 Supertrend + volume delta.

### Major
Parabolic SAR-style (acceleration 0.02, max 0.2) alignment with Supertrend + prior multi-factor (ADX, Williams %R, CCI, MACD-style, BB, VWAP, adaptive RSI/stochastic, MTF). Cap 8%. Vol-scaled. Horizon 8/20.

### Large-cap alt
Breakout + refined volume profile delta imbalance (multi-window accel vs median) + robust volume. Cap 4%.

### Stablecoin
Adaptive depeg watch/alert (30-60/60-90 bp, sustained). Size 0.

### DeFi
Calm regime + Supertrend + volume support. Cap 2%.

### Meme
Qualified burst + volume profile acceleration filter. Cap 0.5%.

### L2
Relative Parabolic SAR excess vs non-stress benchmark + own strength. Cap 3%.

### RWA
Slow Parabolic SAR + adaptive gap/stress halt. Cap 2%. Horizon 24.

### Perpetual
Negative funding + volume delta + contained drift. Cap 2%.

Portfolio correlation regime gate (dynamic threshold) overlays all classes. Size remains volatility-scaled. No live execution.
