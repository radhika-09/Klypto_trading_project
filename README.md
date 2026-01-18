# Klypto_trading_project
**Project Description**

This project is a complete end-to-end implementation of a Regime-Aware Intraday Trading Strategy using Python.
The objective is to design, execute, and evaluate an intraday trading system that adapts to different market regimes instead of applying a single fixed strategy.

The project covers the entire trading pipeline:

1. Data validation
2. Feature engineering
3. Signal generation
4. Position management
5. Strategy return calculation
6. Performance evaluation

**Problem Statement**

1. Traditional intraday strategies often fail because they:
2. Ignore changing market conditions.
3. Generate false signals during sideways markets.
4. Suffer from high drawdowns.

**End-to-End Workflow**

Data Loading & Validation
Load historical intraday market data
Validate required columns
Handle missing values and incorrect data types
Feature Engineering
Calculate technical indicators:
EMA (5-period)
EMA (15-period)
Compute returns
Prepare features for regime detection
Signal Generation
Generate buy/sell signals using EMA crossover logic
Create a signal column based on EMA relationships
Position Management
Convert signals into positions (long / flat)
Shift positions to avoid look-ahead bias
Ensure clean trade execution logic
Strategy Return Calculation
Calculate strategy returns
Remove invalid or zero-return trades
Compute cumulative strategy performance
Regime Awareness
Detect market regimes based on market behavior
Filter trades to execute only in favorable regimes
Reduce overtrading during sideways or noisy markets
Performance Evaluation
Sharpe Ratio
Maximum Drawdown
Total Returns
Win/Loss Ratio
Number of Trades

**Tech Stack**

Language: Python
Libraries Used: pandas, numpy, matplotlib, scikit-learn, technical analysis libraries

**Development Environment:** Jupyter Notebook

**Strategy Logic**

1. Trade direction is decided using EMA crossover.
2. Trades are allowed only when the detected market regime is favorable.
3. Positions are shifted to prevent future data leakage.
4. Performance is measured using professional trading metrics.

**Results & Observations**

1. Reduced false signals compared to basic EMA strategy
2. Improved drawdown control
3. More consistent returns due to regime filtering
4. Cleaner trade execution logic

