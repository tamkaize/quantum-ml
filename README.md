# Quantum Inspired Feature Engineering

## Overview
This project explores how quantum-inspired feature transformations can enhance cross-sectional equity factor models for alpha construction.
We simulate quantum feature maps using Qiskit and apply classical machine learning models to predict relative returns.

---

## Project Structure
- `/data` - Raw and processed stock market data
- `/src` - Core feature engineering, model training, and backtesting code
- `/notebooks` - Experiment notebooks
- `/reports` - Generated charts, metrics, and findings

## Motivation
While quantum computing is not yet practical for live trading, quantum-inspired feature mappings can unlock new representations of financial data. 
This project investigates whether these mappings offer an edge in traditional equity factor modeling and trading.

## Methodology
1. Build the six-factor model proposed by Barillas, Kan, Robotti, and Shanken (2020), which includes: market (Mkt), size (SMB), value with monthly-updated HML following Asness/Frazzini (instead of the traditional annual update by Fama-French), cash-based profitability (RMWc, replacing operating profitability), investment (CMA from the q-factor model), and momentum (UMD). According to the paper *A Comparison of Global Factor Models* by Matthias X. Hanauer (2024), this model achieved an international Sharpe ratio of 2.36.

2. Apply Quantum Kernel Mapping (using Qiskit) to transform features into a higher-dimensional Hilbert space.
   
3. Train classical machine learning models (e.g., SVM, Gradient Boosted Trees) on the quantum-transformed features.
4. 
5. Backtest a long-short equity portfolio strategy based on the predicted cross-sectional alphas.

## Key Technologies
1. Python (Polars, Apache Arrow, Scikit-learn, XGBoost)
2. Qiskit (Quantum Feature Maps, Quantum Kernel Learning)
3. Financial Modeling (Factor Construction, Portfolio Backtesting)

## Results
- Baseline (traditional features only) Sharpe Ratio: In-Progress
- Quantum-augmented feature model Sharpe Ratio: In-Progress
- Cumulative returns chart showing the performance differential.

## Conclusion (In-Progress)
To assess whether quantum-inspired methods offer meaningful improvements in feature expressiveness, further research and live trading validation are needed to evaluate their practical performance—particularly under slippage conditions.

## Acknowledgement
- Barillas et al. six-factor model research


