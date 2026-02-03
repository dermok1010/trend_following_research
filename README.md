# Trend Following Under Realistic Constraints

## Overview
This project investigates whether simple trend-following strategies exhibit statistically robust performance once realistic assumptions are imposed. Rather than optimising for returns, the focus is on methodological correctness, risk behaviour, and failure modes.

The goal of this work is not to claim alpha, but to demonstrate a research-oriented approach to quantitative strategy evaluation: careful data handling, transparent assumptions, and honest validation.

---

## Research Question
Do simple trend-following rules retain economically meaningful signal after accounting for transaction costs, regime dependence, and out-of-sample validation?

---

## Data
Daily price data for liquid equity instruments is used (e.g. SPY).

Key considerations:
- Adjusted prices are used to account for splits and dividends
- Returns are constructed explicitly and justified
- Missing data and non-trading days are handled carefully

Data sources are public and reproducible.

---

## Methodology

### Strategy Definition
A simple time-series trend-following rule is implemented, based on historical price information only. No parameter optimisation is performed in the baseline analysis.

### Backtesting Framework
- Walk-forward (out-of-sample) evaluation
- No look-ahead bias
- Explicit transaction cost assumptions
- Conservative slippage estimates

### Evaluation Metrics
Performance is evaluated using:
- Cumulative returns
- Volatility
- Maximum drawdown
- Drawdown duration
- Tail behaviour

Risk characteristics are prioritised over headline performance metrics.

---

## Regime and Sensitivity Analysis
Strategy behaviour is examined across:
- Different volatility regimes
- Market stress periods
- Alternative parameter choices

This analysis focuses on identifying when and why the strategy fails.

---

## Limitations
- Limited effective sample size
- Results are sensitive to transaction cost assumptions
- Single-asset focus in the baseline implementation

---

## Guiding Principle
This project prioritises methodological rigour and intellectual honesty over performance.
