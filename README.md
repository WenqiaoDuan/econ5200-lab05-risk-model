# econ5200-lab05-risk-model
# Diagnosing a Flawed Risk Model — VaR, Expected Shortfall & Monte Carlo

## Objective

I diagnosed a flawed normal-distribution VaR model and compared different VaR and Expected Shortfall methods while evaluating Monte Carlo simulation accuracy.

## Methodology

* I diagnosed a junior analyst's normal-distribution VaR model and compared its 99% VaR with historical VaR.
* I computed VaR and Expected Shortfall using three methods: historical, normal, and Student-t distributions.
* I fitted a Student-t distribution with 4.58 degrees of freedom.
* I used antithetic variates in the Monte Carlo simulation to reduce the standard error by 1.26x.
* I used the `risk_metrics.py` module and obtained results of 2.7734%, 3.1680%, and 2.7722%.
* I ran the self-tests for the `risk_metrics.py` module.
* I asked an AI to write a VaR backtest, revised my prompt once, and checked the AI-generated result against my own manual count.

## Key Findings

* At the 99% confidence level, the normal-distribution VaR understated historical VaR by 12.7%, or $40,393 on the portfolio.
* The fitted Student-t distribution had 4.58 degrees of freedom.
* Antithetic variates reduced the Monte Carlo standard error by 1.26x.
* The normal 99% VaR was breached on 1.71% of days in the backtest.
* I verified the AI-generated backtest against my own count.
