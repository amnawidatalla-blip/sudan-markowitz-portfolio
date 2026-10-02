# sudan-markowitz-portfolio
Testing a Markowitz-optimized portfolio before vs during the war in Sudan (Python, Google Colab)
# Portfolio Resilience in Sudan's War

Hi, I'm Amna. This is my first coding project, built in Python with Google Colab.

## Goal
Does a portfolio optimized with Markowitz's method on pre-war data (2019 to March 2023) stay resilient during the war in Sudan (April 2023 onward)?

## Data
Sudan's stock market has very little liquid data, so I used 9 global assets as proxies (gold, oil, wheat, US stocks, African stocks, and others) from Yahoo Finance.

## Method
I tested 5,000 random portfolios and picked the one with the best Sharpe ratio before the war. Then I tested its weights on the war period and compared it with an equal-weight portfolio.

## Result
During the war, the optimized portfolio had lower risk (about 9.7%) but a lower Sharpe ratio (about 1.0) than the equal-weight portfolio (about 1.17).

## What I learned
I learned that a portfolio that looks best on past data is not guaranteed to do best in a crisis. In my test, the optimized portfolio had lower risk during the war, but the simple equal-weight portfolio had a better Sharpe ratio. I also saw that small changes, like the random weights or the time period, can noticeably change the results.

## Limitations
Weights come from random search, so results change slightly each run. Sharpe is calculated without a risk-free rate.