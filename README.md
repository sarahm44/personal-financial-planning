# Personal Financial Planning
![Financial Planner](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/financial-planner.png)

## Table of Contents
- [Overview](#overview)
  * [Personal Financial Planner](#personal-financial-planner)
  * [Retirement Planning Tool](#retirement-planning-tool)
- [Financial Planner](#financial-planner)
  * [Collect Crypto Prices](#collect-crypto-prices)
  * [Collect Investments Data](#collect-investments-data)
  * [Perform a Savings Health Analysis](#perform-a-savings-health-analysis)
- [Retirement Planning](#retirement-planning)
  * [Monte Carlo Simulation](#monte-carlo-simulation)
  * [Retirement Analysis](#retirement-analysis)
  * [Early Retirement](#early-retirement)
  
## Overview

This repo includes the following:
1. Personal Financial Planner
2. Retirement Planning Tool

Both analyses are contained in this [financial planner notebook](https://github.com/sarahm44/unit-5-assignment/blob/main/financial-planner.ipynb).

### Personal Financial Planner
A personal finance planner that will allow users to visualize their savings composed by investments in shares and cryptocurrencies to assess if they have enough money as an emergency fund.

### Retirement Planning Tool
A retirement planning tool that will use the [Alpaca API](https://alpaca.markets/) to fetch historical closing prices for a retirement portfolio composed of stocks and bonds, then run Monte Carlo simulations to project the portfolio performance at 30 years. 

The Monte Carlo data will be used to calculate the expected portfolio returns given a specific initial investment amount.

## Financial Planner
The elements of the Financial Planner are set out below.

### Collect Crypto Prices

I collected crypto prices for BTC and ETH from [Alternative Free Crypto API](https://alternative.me/crypto/api/) using the requests Library:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/crypto_prices.png)

### Collect Investments Data

I collected investments data using [Alpaca API](https://alpaca.markets/) for SPY (stocks) and AGG (bonds):

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/investment_data.png)

### Perform a Savings Health Analysis

First I created a DataFrame containing the amount of crypto assets and shares:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/dataframe.png)

Then I visualised this as a pie chart:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/pie_chart.png)

Based on a monthly income of $12,000, I used `if` conditional statements to validate if the current savings are enough for an emergency fund. It was assumed that an ideal emergency fund should be equal to three times your monthly income:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/if_statement.png)

## Retirement Planning

### Monte Carlo Simulation
I collected 5 years of historical investments data using [Alpaca API](https://alpaca.markets/) for SPY (stocks) and AGG (bonds):

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/historical_data.png)

Then I ran a Monte Carlo simulation to forecast 30 years cumulative returns with 500 runs, and plotted the outcome:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/mc_sim.png)

See below a plot of the probability distribution and confidence intervals:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/probability_distribution.png)

The summary statistics or the Monte Carlo simulation are set out below:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/mc_statistics.png)


### Retirement Analysis

I calculated the expected portfolio return at the 95% lower and upper confidence intervals based on a $20,000 initial investment:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/20k_increase.png)

I calculated the expected portfolio return at the 95% lower and upper confidence intervals based on a 50% increase in the initial investment:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/50pc_increase.png)

### Early Retirement

The five year retirement option Monte Carlo simulation result is as follows:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/5_years.png)

The ten year retirement option Monte Carlo simulation result is as follows:

![""](https://github.com/sarahm44/unit-5-assignment/blob/main/Images/10_years.png)
