# A Comprehensive Cointegration-Based Forex Pair Trading Strategy: Utilizing Stationarity Tests, Engle-Granger Method, and OLS Regression for Trade Execution

## Overview

This project implements a Forex pair trading strategy leveraging cointegration to identify profitable trading opportunities. Forex pair trading involves trading two non-stationary (non-mean-reverting) currency pairs, with the trading position based on their relative movements. A cointegration-based approach ensures that the spread between the pair is mean-reverting, offering profitable trading opportunities.

The strategy employs stationarity tests to confirm the non-stationarity of the pairs, the Engle-Granger method to confirm cointegration, and Ordinary Least Squares (OLS) regression to calculate the spread. This spread is then used to make trade decisions.

## Project Steps

1. **Data Fetching**
   - Data for 14 major  currencies were fetched using the `yfinance` library.
   
2. **Stationarity Tests**
   - Conducted Augmented Dickey-Fuller (ADF) tests to confirm the non-stationarity of the currency pairs, a prerequisite for pair trading.

3. **Engle-Granger Cointegration Test**
   - Applied the Engle-Granger test to confirm cointegration between the non-stationary pairs.

4. **Ordinary Least Squares (OLS) Regression**
   - Used OLS regression to find the spread between cointegrated pairs, which will be used for trade decision-making.

5. **Cumulative Returns Calculation**
   - Calculated cumulative returns for the cointegrated pairs to evaluate the performance of the trading strategy.

## Setup and Usage

### Prerequisites

- Python 3.x
- `yfinance` library
- `statsmodels` library
- `pandas` library
- `numpy` library
- `matplotlib` library

### Installation

Install the required Python packages:

   ```sh
   pip install yfinance statsmodels pandas numpy matplotlib
   ```

### Running the Strategy

1. **Fetch Data:**

   Run the script to fetch historical data for the 14 currencies using `yfinance`.

2. **Stationarity Tests:**

   Execute the script to perform stationarity tests (ADF tests) on the currency data to confirm non-stationarity.
   
4. **Engle-Granger Cointegration Test:**

   Run the script to perform the Engle-Granger test to confirm cointegration between the non-stationary pairs.
   
6. **OLS Regression:**

   Perform OLS regression to calculate the spread between the cointegrated pairs.

7. **Cumulative Returns Calculation:**

   Calculate and plot cumulative returns for the cointegrated pairs to evaluate the performance of the trading strategy.

## Files and Directories

- `Data_fetch.py`: Script to fetch historical currency data.
- `ADF_test.py`: Script to perform stationarity tests.
- `cointegration_test.py`: Script to perform Engle-Granger cointegration tests.
- `spread_signal.py`: Script to perform OLS regression to find spreads.
- `cal_returns.py`: Script to calculate and plot cumulative returns.

## Notes

- Ensure you have an active internet connection to fetch data using `yfinance`.
- Review the outputs of each script to ensure the data and tests are executed correctly.
- Adjust the scripts as necessary to fit your specific requirements and trading parameters.

## Conclusion

This project provides a comprehensive framework for implementing a cointegration-based Forex pair trading strategy. By leveraging statistical tests and regression analysis, it identifies trading opportunities based on mean-reverting spreads between cointegrated currency pairs.
