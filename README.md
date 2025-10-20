# Contextual Multi-Bar Engulfing Engine

A precision-focused Pine Script indicator for detecting high-quality bullish and bearish engulfing patterns. Designed for strict compliance, adaptive filtering, and multi-timeframe validation—ideal for FX and crypto traders seeking robust setup detection.

##  Features
- Detects 2-bar and 3-bar engulfing clusters
- Filters by ADX strength and EMA slope
- Validates trend alignment on higher timeframes
- Adaptive volume trap logic based on session volatility
- Candle quality filters: body size, wick ratio, overlap, inside bars
- Scoring system to rank setup strength
- Optional debugging tools for signal validation

##  Inputs
- `ADX Length`, `ADX Threshold`: trend strength filters
- `Fast EMA`, `Slow EMA`: slope-based trend direction
- `Higher Timeframe`: for confluence validation
- `Min Body %`, `Max Wick Ratio`: candle quality thresholds
- `Score Min`: minimum score required to show signal
- `Show Debug`: toggle for internal signal diagnostics

##  Signals
-  Green triangle: 2-bar bullish engulfing
-  Red triangle: 2-bar bearish engulfing
-  Lime circle: 3-bar bullish engulfing
-  Maroon circle: 3-bar bearish engulfing

##  Debug Mode
Enable `Show Debug` to visualize:
- Normalized setup score
- Raw engulfing flags
- Invalidation triggers

##  Usage
1. Add the script to a TradingView chart.
2. Select your preferred timeframe (e.g., 15m, 1h).
3. Adjust inputs to match your strategy and asset volatility.
4. Use visual signals and score plot to identify high-confidence setups.
5. Enable debug mode for deeper analysis and refinement.

---

**Note:** This engine is optimized for real-time detection and strict invalidation. For parity testing or automation, consider extending to Python or NinjaTrader.

