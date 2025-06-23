# Algorithmic-Quant-Trading-Strategy-
A Python-based quant strategy using technical indicators, portfolio optimization, and performance analysis.

This project implements a systematic, data-driven algorithmic trading strategy built with Python. It combines historical market data, technical indicators, clustering, and modern portfolio theory to generate dynamic asset allocations and improve investment outcomes.

Features
- Calculates historical asset returns and volatility
- Uses PyPortfolioOpt to construct optimized portfolios
- Integrates unsupervised learning (e.g., clustering) to group assets
- Dynamically adjusts allocations over time
- Compares against benchmark indices like SPY (Buy & Hold)
- Evaluates Sharpe Ratio, Max Drawdown, and other key metrics
- Provides visualizations of cumulative returns and volatility

Technical Indicators Used

This strategy extracts and uses the following technical indicators for signal generation and portfolio decision-making:

- **Garman-Klass Volatility** – more accurate volatility estimator than simple close-to-close returns
- **RSI (Relative Strength Index)** – measures momentum and potential overbought/oversold conditions
- **Bollinger Bands (BBANDS)** – identifies volatility and price levels relative to recent averages
- **ATR (Average True Range)** – captures market volatility
- **MACD (Moving Average Convergence Divergence)** – trend-following momentum indicator
- **Volume** – used as a filter and confirmation signal

Includes data preprocessing, strategy logic, performance evaluation, and visualizations.

![image](https://github.com/user-attachments/assets/712f6ce0-3209-4573-a399-bd706a7de364)

The plot compares cumulative returns of the custom "Unsup Trading Strategy" (in red) vs SPY Buy & Hold (in blue) from 2016 to 2025.
The strategy not only outperforms in overall return (~190% vs ~145%), but also shows lower drawdowns during turbulent periods like 2020 and 2021, indicating better downside protection and risk management.


This algorithmic trading strategy achieved an annualized return of 14.98% with a Sharpe ratio of 0.798, outperforming the S&P 500's Sharpe ratio of 0.72. Despite a slightly higher volatility (18.77% vs. 11.98%), the strategy delivers superior risk-adjusted returns compared to a passive buy-and-hold approach. This indicates more efficient capital allocation and better downside protection during drawdowns.

Performance Summary

| Metric                 | Strategy        | S&P 500 (Benchmark) |
|------------------------|-----------------|----------------------|
| Annualized Return      | **14.98%**       | ~13.0%               |
| Annualized Volatility  | 18.77%           | 11.98%               |
| Sharpe Ratio           | **0.798**        | 0.72                 |
| Max Drawdown           | -32.0%           | -13.9% (avg intra-year) |


Future Improvements

- Reduce drawdown through volatility targeting or stop-loss logic
- Incorporate fundamental features (e.g., earnings growth)
- Test with different clustering algorithms (DBSCAN, KMeans++)
- Add walk-forward optimization
- Extend to international assets or crypto markets
