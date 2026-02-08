# Quantitative Asset Research (2025)

This repository contains professional-grade financial models developed to analyze market risk and algorithmic trading strategies.

## Project 1: Multi-Asset Correlation Analysis
* **Goal:** Use Pearson Correlation to identify diversification benefits across US Equities, Aussie Equities, Gold, and Crypto.
* **Math:** Calculated Log-Returns to ensure statistical stationarity.
* **Result:** Successfully mapped the decoupling of BTC-USD from traditional safe-havens like Gold in late 2025.

## Project 2: Apple (AAPL) Momentum Strategy
* **Methodology:** Developed a 50/200-day Simple Moving Average (SMA) crossover backtest.
* **Risk Metrics:** Achieved an **Annualized Sharpe Ratio of 0.86**.
* **Drawdown:** Identified a **Maximum Drawdown of -24.58%**, highlighting the strategy's volatility during market shifts.

## Project 3: Risk-Parity Engine (Diversified Fund)
* **Goal:** Solve the high drawdown issues found in Project 1.
* **Math Strategy:** Used **Inverse Volatility Weighting** ($1/\sigma$) to equalize risk across SPY, VAS.AX, Gold, and Bitcoin.

### Project 3 Final Audit
* **Total Return:** 40.99%
* **Max Drawdown:** -3.66% (Extremely low risk)
* **Sharpe Ratio:** 1.61 (Professional grade risk-adjusted return)
* **Logic:** Proved that Inverse-Volatility weighting can capture Bitcoin's upside while using Bonds/Gold to crush the downside.

![image](./assets/portfolio_growth.png)

### 04 | Institutional Risk Engine (VaR/CVaR & Monte Carlo)
* **Core Tech:** Python, `yfinance`, `scipy.stats`, Monte Carlo Simulation.
* **The Problem:** Standard metrics (Sharpe Ratio) often hide "Black Swan" risks in Crypto/Tech portfolios.
* **The Solution:** Built a multi-model engine to calculate **95% Value at Risk** and **Expected Shortfall**, identifying a 3.30% average crash depth.
* **Links:** [View Notebook](./04_Risk_Modeling/Risk_Modeling.ipynb) | [Live Colab Dashboard](https://colab.research.google.com/github/RyanSVargas/Quant-Finance-Research/blob/main/04_Risk_Modeling/Risk_Modeling.ipynb)
