# Portfolio Analysis: Equal-Weighted, Value-Weighted & Portfolio Optimization

## Overview
This project demonstrates **portfolio construction and optimization** using historical stock data. It explores two portfolio strategies : **equal-weighted** and **value-weighted** and performs **portfolio optimization** on a subset of stocks using mean-variance analysis and the efficient frontier.  

The goal is to compare **risk-return characteristics**, **growth patterns**, and **risk-adjusted performance** for different portfolio strategies.

## Data
- **Source:** Yahoo Finance  
- **Stocks (Part 1):** AAPL, MSFT, AMZN, NVDA, JPM, GOOGL, TSLA, META  
- **Stocks (Part 2 - Optimization):** TSLA, JNJ  
- **Period:** Jan 2021 – Sep 2025  
- **Frequency:** Monthly adjusted closing prices  

## Part 1: Buy-and-Hold Portfolio Construction
### Methodology
- **Equal-Weighted Portfolio:** Each stock receives an equal proportion of the initial investment.  
- **Value-Weighted Portfolio:** Weighting based on simulated market capitalization (larger-cap stocks carry higher weights).  
- **Portfolio Value:** Calculated at month-end without rebalancing.  
- **CAGR:** Computed for annualized growth.

### Results
- **Equal-Weighted Portfolio:** Early growth slightly faster due to higher exposure to smaller-cap stocks but more volatile.  
- **Value-Weighted Portfolio:** More stable growth; larger-cap stocks dominate performance over time.

**CAGR Example:**
| Portfolio          | CAGR   |
|------------------|--------|
| Equal-Weighted    | 0.13   |
| Value-Weighted    | 0.14   |

### Visualization
- **Cumulative Portfolio Value:** Equal-weighted vs Value-weighted  

**Interpretation:**  
Equal-weighted portfolios capture early gains from smaller stocks but are more sensitive to volatility. Value-weighted portfolios grow steadily, driven by larger stocks, and are generally more stable over time.  

## Part 2: Portfolio Optimization
### Methodology
- **Stocks:** TSLA and JNJ  
- **Returns:** Monthly discrete returns  
- **Optimization:** Mean-variance analysis  
  - Minimum-Variance Portfolio (MVP)  
  - Optimal Risky Portfolio (max Sharpe ratio)  
- **Efficient Frontier:** Visual representation of risk-return trade-off

### Results
| Portfolio Type         | TSLA Weight | JNJ Weight | Expected Annual Return | Portfolio Risk (σ) |
|-----------------------|------------|------------|-----------------------|------------------|
| Minimum-Variance       | 9.2%       | 90.8%      | 9.3%                  | 15.2%            |
| Optimal Risky          | 100%       | 0%         | 32.1%                 | 64.9%            |

### Visualization
- **Efficient Frontier Plot:** Shows achievable portfolios, highlighting MVP (lowest risk) and Optimal Risky Portfolio (highest Sharpe ratio)  

**Interpretation:**  
- MVP prioritizes **stability with moderate returns** suitable for risk-averse investors.  
- Optimal Risky Portfolio maximizes **risk-adjusted returns**, ideal for investors willing to take higher risk.  
- The plot highlights the trade-off between risk and return, guiding strategic portfolio allocation decisions.

## Key Insights
- Equal-weighted vs value-weighted portfolios demonstrate the impact of stock weighting on portfolio growth and volatility.  
- Portfolio optimization with mean-variance analysis identifies **efficient portfolios** along the frontier, balancing return and risk.  
- Investors can use the **minimum-variance portfolio** for stability or the **optimal risky portfolio** for higher risk-adjusted returns.

