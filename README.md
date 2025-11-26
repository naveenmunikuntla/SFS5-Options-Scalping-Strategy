# Smart Flow Scalper (SFS-5) Strategy

**Version 1.0 - November 26, 2025**

## Overview

**Smart Flow Scalper (SFS-5)** is a systematic 5-factor naked options intraday scalping strategy designed for NIFTY weekly options. Created for non-technical traders with focus on risk management and automation via Perplexity Labs.

### Key Features
- ✅ 5-Factor entry system (VWAP, Volume, RSI, OI, VIX)
- ✅ Strict risk management (2% per trade, 4% daily limit)
- ✅ Time-based exits (20-60 min max hold)
- ✅ Designed for automation (Perplexity Labs ready)
- ✅ Current market specs (Nov 2025: NIFTY lot=75, Tuesday expiry)

### Strategy Specifications

| Parameter | Value |
|-----------|-------|
| **Strategy Type** | Naked Options Buying |
| **Timeframe** | 5-minute |
| **Instrument** | NIFTY Weekly Options (NSE) |
| **Hold Time** | 20-60 minutes |
| **Capital Required** | ₹1,00,000 - ₹3,00,000 |
| **Expected Win Rate** | 50-55% |
| **Monthly Returns** | 25-40% |
| **Max Drawdown** | 12-15% |
| **Risk per Trade** | 2% |

### Current Market Parameters (Nov 26, 2025)

- **NIFTY Lot Size**: 75 (changes to 65 on Dec 30, 2025)
- **Weekly Expiry**: Every TUESDAY
- **Trading Days**: Wednesday, Thursday, Friday only
- **Avoid**: Monday-Tuesday (expiry week volatility)
- **API**: FYERS V3 (version 3.3.6)

### The 5 Factors

1. **VWAP (30% weight)**: Trend direction filter
2. **Volume Spike (25% weight)**: Momentum confirmation (>2x average)
3. **RSI (20% weight)**: Momentum shift (50-level crossover)
4. **Open Interest (15% weight)**: Institutional positioning
5. **India VIX (10% weight)**: Volatility environment (12-18 optimal)

### Entry Rules

**CALL Buying**: Price > VWAP, Volume >2x, RSI crosses above 50, VIX 12-18
**PUT Buying**: Price < VWAP, Volume >2x, RSI crosses below 50, VIX 12-18

### Risk Management

- **Stop Loss**: 25-30% premium loss OR technical/time stop
- **Targets**: 30-40% (exit 50%), 60-80% (exit 30%)
- **Daily Limit**: Max 4-5 trades, 4% loss limit
- **Weekly Limit**: 8% loss limit

## Files in This Repository

### Core Documentation
1. **SFS5_Strategy_Master_Document.csv** - Complete 12-section strategy overview
2. **SFS5_Perplexity_Labs_Prompts.csv** - 4 essential prompts for building tools
3. **SFS5_Comparison_Framework.csv** - Template to evaluate external strategies

### Analysis Files
4. **naked_options_scalping_strategy.csv** - Detailed entry/exit rules
5. **naked_options_expected_performance.csv** - Performance targets
6. **updated_position_sizing_nov2025.csv** - Current lot sizes & calculations

### Reference Files
7. **options_scalping_factors_analysis.csv** - 12-factor deep dive
8. **strategy_entry_exit_rules.csv** - Entry/exit documentation
9. **strategy_implementation_roadmap.csv** - 5-phase timeline

## Quick Start

### Using Perplexity Labs (Recommended)

1. Open `SFS5_Perplexity_Labs_Prompts.csv`
2. Copy Prompt 1 (Dashboard) or Prompt 2 (Backtest)
3. Paste into Perplexity Labs
4. Labs will generate complete code in 10-15 minutes

### Implementation Timeline

- **Week 1**: Setup & Paper Trading
- **Week 2**: Live Trading (1 lot)
- **Week 3-4**: Build Consistency (2 lots after 20 wins)
- **Month 2-3**: Scale Up
- **Month 4+**: Full Capital Allocation

## Important Notes

⚠️ **CRITICAL UPDATES**:
- NIFTY expiry moved to **TUESDAY** (not Thursday) as of Sept 2025
- BANKNIFTY has **NO weekly expiries** (monthly only)
- SENSEX unsuitable for scalping (low liquidity)
- NIFTY lot size **75 → 65** on December 30, 2025

## Performance Expectations

### Moderate Trader (₹2,00,000 capital)
- Daily target: 4-6% (₹8,000-₹12,000)
- Monthly returns: 25-40% (₹50,000-₹80,000)
- Max drawdown: 12-15%
- Trades per day: 3-4
- Risk-reward: 1:2

## Disclaimer

This strategy is for educational purposes. Options trading involves substantial risk. Past performance does not guarantee future results. Trade at your own risk.

## Author

Developed by Naveen (48 years, Full-time Trader, Hyderabad)
Created with Perplexity Labs on November 26, 2025

---

**License**: MIT
**Questions**: Open an issue in this repository