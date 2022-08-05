# Personal Financial Planning
![Financial Planner](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/financial-planner.jpg)

## Overview

This activity involves two tasks:
1. Personal Financial Planner
2. Retirement Planning Tool

### Personal Financial Planner
A personal finance planner that will allow users to visualize their savings composed by investments in shares and cryptocurrencies to assess if they have enough money as an emergency fund.

### Retirement Planning Tool
A retirement planning tool that will use the [Alpaca API](https://alpaca.markets/) to fetch historical closing prices for a retirement portfolio composed of stocks and bonds, then run Monte Carlo simulations to project the portfolio performance at 30 years. 

The Monte Carlo data will be used to calculate the expected portfolio returns given a specific initial investment amount.

## Financial Planner
The tasks required for the Financial Planner are set out below.

### Collect Crypto Prices

I collected crypto prices for BTC and ETH from [Alternative Free Crypto API](https://alternative.me/crypto/api/) using the requests Library.

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/financial-planner.jpg)

### Collect Investments Data

I collected investments data using [Alpaca API](https://alpaca.markets/) for SPY (stocks) and AGG (bonds).

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/financial-planner.jpg)

### Perform a Savings Health Analysis

First I created a DataFrame containing the amount of crypto assets and shares.

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/financial-planner.jpg)

I visualised this as a pie chart.

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/financial-planner.jpg)

Based on a monthly income of $12,000, I used 'if' conditional statements to validate if the current savings are enough for an emergency fund. It was assumed that an ideal emergency fund should be equal to three times your monthly income.

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/financial-planner.jpg)
