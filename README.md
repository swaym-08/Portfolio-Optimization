# Portfolio Optimization with GARCH Volatility Forecasting

## Overview
This project focuses on portfolio optimization using a Generalized Autoregressive Conditional Heteroskedasticity (GARCH) model to forecast volatility for a set of assets. The project leverages GARCH models to estimate the conditional volatility of asset returns, which are then used to calculate a covariance matrix for portfolio optimization. The primary goal is to maximize the Sharpe ratio of a portfolio by selecting optimal asset weights based on historical return data.

## Key Features
### GARCH Model Volatility Forecasting:

The project fits GARCH models to asset return data (log returns) to estimate future volatility.
Volatility predictions are used as a key input to portfolio optimization.
The model is capable of handling multiple assets and can compute volatility for each asset individually.
### Portfolio Optimization:

Portfolio weights are optimized to minimize risk (variance) or to maximize the Sharpe ratio.
Constraints ensure that the portfolio weights sum to 1, and the portfolio is long-only (no short positions).
The portfolio’s risk is evaluated using the covariance matrix calculated from asset volatilities and correlations.
### Expected Returns and Volatility:

The project calculates mean returns and annualized volatility for assets, using historical price data.
The conditional volatility estimated by the GARCH model can be annualized to provide long-term risk estimates.
### Optimizing the Sharpe Ratio:

The project uses optimization techniques to find the portfolio with the highest Sharpe ratio (risk-adjusted return).
This optimization is based on asset returns, volatilities, and correlations.
