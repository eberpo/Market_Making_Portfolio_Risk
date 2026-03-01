# OTC Option Portfolio: Hedging and Risk Analysis

This repository contains a  Jupyter notebook that builds and analyzes an OTC options portfolio on **Walt Disney Co. (DIS)** for the business day **Nov 12, 2025**. Notebook covers data loading, option pricing, implied volatility estimation, portfolio construction, risk shocks, historical risk metrics, and stress testing.

## Contents

* **Data gathering & selection**

  * Equity/stock data, listed options data, chosen business day filters
  * Risk-free rate curve construction and interpolation
* **Pricing framework**

  * Option and portfolio constructors
  * Pricing and Greeks computation with Black–Scholes setup and curve inputs
* **Market data**

  * Eligible listed options filtering
  * Implied volatility calculation for the market surface
* **Strategy**

  * Strategy classes and a structured OTC portfolio split into blocks
  * Selection of listed options for hedging/implementation
* **Portfolio risk analysis**

  * Portfolio composition and payoff/shape visualization
  * Shock scenarios applied to option and stock components
  * **Historical VaR / ES** (1-day and 5-day adjusted)
  * Strategy P&L analysis and **stress test**

## Repository structure

* `Notebook.ipynb` — main analysis notebook
* `data/` — required input files:

  * `DIS.xlsx`
  * `Equity.xlsx`
  * `Risk_Free.xlsx`
  * `VIX.xlsx`

