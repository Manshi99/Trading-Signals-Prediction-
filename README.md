# Trading-Signals-Prediction
MSBA Capstone Project with Spinnaker Analytics

Team 14 members: Tzuhua(Agnes) Huang, Ziqi Shan, Kangjing Shi, Man Shi

## Purpose
The objective of the project is to find tradable signals across sectors for helping investor to identify ‘sector-rotation patterns’ in financial markets and develop tradable predictions.


## Dataset
* The dataset contains sectoral data for 3 separate types of investments made in the US: Institutional Mutual Fund, Institutional ETF, and Retail Mutual Fund. 
* The weekly data spans 10 years from 2006 through end-Jan 2017. Not all sectors have data available for all the dates since new investment vehicles are introduced at various points in time.

## Data Fields
* ReportDate: Weekly data aggregated and released every Wednesday
* AssetClass: Industry/Sector/Asset Class
* Flow: Amount of positive (inflow) or negative (outflow) in Millions of USD
* FlowPct: Flows as percent of assets at beginning of the week
* AssetsEnd: Assets at end of the week in Millions of USD
* PortfolioChangePct: Percent change in overall portfolio during the week

## Outline
* Notebook 1 - Data Cleaning + EDA + VAR Model 1 ([Open with Google Colaboratory](https://colab.research.google.com/drive/1Cmi1CiAxu6D5MqBYdtGjX3OHQPBtqIfo?usp=sharing))

  1. Data cleaning
  2. Explanatory data analysis
  3. VAR Model 1-1: Within one market - ETF
  4. VAR Model 1-2: Within one market - Institutional MF

* Notebook 2 - VAR Model 2 ([Open with Google Colaboratory](https://colab.research.google.com/drive/19HYToVdgtO8F053-4ustfHvKujie9yyT?usp=sharing))

  5. VAR Model 2-1: Cross-market
  6. VAR Model 2-2: Cross-market, smoothing method (Moving Average) applied

* Notebook 3 - VAR Model 3 ([Open with Google Colaboratory](https://colab.research.google.com/drive/1ziqzM5N4ULgjuEz_scKYggixpPQkdfKd?usp=sharing))

  7. VAR Model 3: Cross-market, smoothing method (Moving Average) applied and market indices added

## Key findings
* Changing the actual value to be a directional number could highly improve our prediction.
* Applying smoothing method and add additional market index variable could both increase model accuracy. 
