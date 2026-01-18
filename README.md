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

1. Data Loading & Validation
2. Load historical intraday market data
3. Validate required columns
4. Handle missing values and incorrect data types
5. Feature Engineering
6. Calculate technical indicators:
7. EMA (5-period)
8. EMA (15-period)
9. Compute returns
10. Prepare features for regime detection
11. Signal Generation
12. Generate buy/sell signals using EMA crossover logic
13. Create a signal column based on EMA relationships
14. Position Management
15. Convert signals into positions (long / flat)
16. Shift positions to avoid look-ahead bias
17. Ensure clean trade execution logic
18. Strategy Return Calculation
19. Calculate strategy returns
20. Remove invalid or zero-return trades
21. Compute cumulative strategy performance
22. Regime Awareness
23. Detect market regimes based on market behavior
24. Filter trades to execute only in favorable regimes
25. Reduce overtrading during sideways or noisy markets
26. Performance Evaluation
27. Sharpe Ratio
28. Maximum Drawdown
29. Total Returns
30. Win/Loss Ratio
31. Number of Trades

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

