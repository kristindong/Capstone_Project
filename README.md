# Capstone_Project
Final Project for Data Analytics Class: Financial Indicators vs Stock Market Performance

## Overview

[Link to Google Slides](https://docs.google.com/presentation/d/1rg12WplVf4fy3VU82EIZb64H5yveYUukMScgsefe0KI)

The allure of better understanding the relationship between a company’s financial data and it's stock market performance is obvious. The market may seem chaotic, but with enough data can we reasonably predict a company's performance? Can we determine which factors are significantly tied to a stocks performance? Aided by the knowledge gained in this course we can attempt engage these questions. 

Our data set is composed of over 200 key financial indicators typically found in annual the 10-k fillings from roughly 4000 companies for the years 2014 - 2018. Though voluminous, the data set in neither complete (there are some null values) nor perfect (there are some suspicious outliers) and will require some cleaning. We sourced our data from [Kaggle's repository](https://www.kaggle.com/datasets/cnic92/200-financial-indicators-of-us-stocks-20142018) 

With this data and our sophisticated analysis, we hope to determine if it is possible to predict the performance of a stock (as measured by whether the stock price increased or decreased in one calendar year) from key financial indicators and if so, which indicators are the most strongly tied to a company’s performance. 

As there are over 200 indicators in the original data set, many of which are redundant or overlap, we selected a subset of indicators that are considered to be most relevant for our model:

1. Gross Profit Margin = (Revenue - Cost of Sales) / Revenue * 100
2. Net Profit Margin = Net Profit / Revenue * 100
3. Working Capital = Current Assets - Current Liabilities
4. Current Ratio = Current Assets / Current Liabilities
5. Quick Ratio = (Current Assets - Inventory) / Current Liabilities
6. Leverage = Total Assets / Total Equity
7. Debt to Equity Ratio = Total Debt / Total Equity
8. Inventory Turnover = Cost of Sales / (Beginning Inventory + Ending Inventory / 2)
9. Total Asset Turnover = Revenue / (Beginning Total Assets + Ending Total Assets / 2)
10. Return on Equity (ROE) = Net Profit / (Beginning Equity + Ending Equity) / 2
11. Return on Assets (ROA) = Net Profit / (Beginning Total Assets + Ending Total Assets) / 2
12. Operating cash flow
13. Earnings per Share (EPS)
14. Price-Earnings Ratio (P/E)
15. EBITDA
16. Free cash flow
17. Sector
18. R&D expense

