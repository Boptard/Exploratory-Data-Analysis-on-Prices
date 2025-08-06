# Quantitative EDA on Large-Cap Tech Equities

A structured exploratory data analysis (EDA) pipeline for AAPL, GOOG, and MSFT that cleanly ingests price & volume data, computes and visualizes key metrics, uncovers seasonal and risk patterns, estimates market betas, and assembles a comprehensive feature matrix for downstream modeling or backtesting.

---

## 📈 Project Overview

1. **Data Ingestion & Cleaning**  
   • Downloaded daily OHLC and volume via Yahoo Finance  
   • Handled missing data, aligned business-day indices  
2. **Descriptive Statistics & Returns**  
   • Computed simple vs. log returns  
   • Generated summary tables (mean, σ, quantiles)  
3. **Time-Series Visualizations**  
   • Price vs. 20-day moving average  
   • Rolling 20-day annualized volatility  
   • Max drawdowns & underwater curves  
4. **Correlation & Seasonality**  
   • Return correlation heatmaps  
   • Weekday & month-of-year average returns  
5. **Volume–Return Analysis**  
   • Scatterplots and histograms of volume vs. returns  
   • Quantified correlation between volume spikes and large moves  
6. **CAPM Beta Estimation**  
   • Regressed against S&P 500 to extract α, β, and R² using NumPy’s `polyfit`  
7. **Momentum Indicator**  
   • Computed 14-day RSI to highlight overbought/oversold regimes  
8. **Feature Matrix Construction**  
   • Consolidated all signals (returns, MA, vol, RSI) for modeling  
