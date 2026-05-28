# TPAAM — Thematic Probabilistic Asymmetry Allocation Model

An 8-layer, regime-aware capital allocation framework for identifying and sizing asymmetric investment opportunities.

## Quick Start

```bash
python3 tactical/tactical_tpaam.py --scan
python3 tactical/tactical_tpaam.py --check XCUUSD
```

## System Architecture

**8 Layers:**
1. Regime Detection (6 market regimes from 9 macro indicators)
2. Theme Discovery (10 structural themes with adoption curves)
3. Asymmetry Engine (probability × magnitude optimization)
4. Multi-Factor Scoring (Q/V/N/A/P/T dynamic weighting)
5. Dynamic Weighting (regime-adaptive factor weights)
6. Position Sizing (conviction + volatility + regime modifiers)
7. Portfolio Construction (concentration + correlation constraints)
8. Feedback Loop (IC-based weight refinement)

## Live Validation Results

19 trades across FTMO forex/metals, crypto, NIFTY options:
- **System compliance win rate:** 64.3% (when fully followed)
- **Override win rate:** 0% (rule violations)
- **MTA (multi-timeframe alignment) IC:** +0.632 (strong predictor)
- **HTF confirmed trades:** 83% win rate | Unconfirmed: 20%

## Key Insights

1. **Execution discipline >> model sophistication** — Following system rules produces 64.3% wins; overriding produces 0% wins.
2. **MTA is the strongest predictor** — Daily chart alignment (HTF confirmation) yields 4x win rate multiplier.
3. **Regime-adaptive weighting works** — Factor importance shifts dramatically across market regimes (quality dominates panic, narrative dominates mania).
4. **Early narrative > late narrative** — Positioning at narrative acceleration (velocity > +0.35) vs saturation (velocity < -0.35) determines asymmetry quality.

## Files

- `tpaam/` — Core 8-layer modules
- `tactical/` — Execution interface (scanner, trade logger, config)
- `TPAAM_Living_Document_v1_1.md` — Full system specification
- `tactical/EXAMPLE_TRADE_LOG.csv` — Sample trade log format

## Author

Rahul Sai Boddapati | boddapati.rahul@gmail.com
