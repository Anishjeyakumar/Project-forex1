# A Comprehensive Cointegration-Based Forex Pair Trading Strategy: Utilizing Stationarity Tests, Engle-Granger Method, and OLS Regression for Trade Execution 

## Overview

Forex pair trading involves trading two non stationary(Non mean reverting) currency pair whose spread decides the trading position based on their relative movements
. A cointegration-based approach ensures that the spread between the pair are mean-reverting which offers profitable trading opportunities. This strategy will employ 
stationarity tests to confirm the Non- stationarity of the pairs ,cointegrity between the pair is confirmed using the Engle-Granger method, and the spread will be calculated using Ordinary Least Squares (OLS) regression which ensure trading opportunities
based on the spread between two non stationary currencies

##Outline:

## 1. Data Collection:

    Price data of about 14 major currencies we fetched using Yfinance library
