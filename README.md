# Capstone_Project
Final Project for Data Analytics Class: Using Common Financial Indicators to Predict Stock Performance

## Overview

[Link to Google Slides](https://docs.google.com/presentation/d/1rg12WplVf4fy3VU82EIZb64H5yveYUukMScgsefe0KI)

The allure of better understanding the relationship between a company’s financial data and it's stock market performance is obvious. The market may seem chaotic, but with enough data can we reasonably predict a company's performance? Can we determine which factors are significantly tied to a stocks performance? Aided by the knowledge gained in this course we can attempt engage these questions.

- Identify and assess a suitable data set
- Clean, prepare, and explore data
- Analysis
- Dashboard and Data Story

With data and our sophisticated tools and analysis, we hope to determine if it is possible to predict the performance of a stock (as measured by whether the stock price increased or decreased in one calendar year) from key financial indicators and if so, which indicators are the most strongly tied to a company’s performance and to be able to present our finding in an understandable way.


## Data

### Source and Description

The data was sourced from Kaggle's data repository [Kaggle's repository](https://www.kaggle.com/datasets/cnic92/200-financial-indicators-of-us-stocks-20142018). The full data set consisted of four files containing over 200 key financial indicators typically found in annual 10-k fillings from roughly 4000 companies for the years 2014 - 2018. In addition to the financial indicators, the data contained price variance variable, defined as the percentage change in the stock's price over the calendar year), and a class variable with the label "1" if the price increased and "0" otherwise. For this analysis we focused only on the 2018 data set. 

### Data Exploration

During preliminary data exploration, it was apparent that the data contained null values and suspicious values (for example, values falling outside of expected range). In addition, there were redundant variables (multiple columns of the same variable) and many variables that had some overlapping (for example, gross profit and net profit).
 
To make data processing and model training more efficient, we selected and kept only a subset of variables that are commonly considered to be most indicative of company performance. The following variables were kept in the data:

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
19. Class



Creating two tables 

Data cleaning

[stock_prediction_seg2_v6.ipynb](https://github.com/kristindong/Capstone_Project/blob/main/stock_prediction_seg2_v6.ipynb)

- We created a sqlite database with two tables in it: 
  - Features
  - Target 
- We tested querying the database
- We linked the two tables
- We joined the tables using our primary keys
- Encoding certain columns to prepare it for machine learning
- We dropped null values and unnecessary columns
- We also used session.query to create sessions

## Analysis
✓ Description of data preprocessing
✓ Description of feature engineering and the feature selection, including their decision- making process
✓ Description of how data was split into training and testing sets
✓ Explanation of model choice, including limitations and benefits
✓ Explanation of changes in model choice (if changes occurred between the Segment 2 and Segment 3 deliverables)
✓ Description of how they have trained the model thus far, and any additional training that will take place
✓ Description of current accuracy score

## Technologies and Tools

- Excel
- Jupyter Notebook
- Python, including the following libraries:
  - Pandas
  - Matplotlib
  - Sqlalchemy
  - Scikit-learn
  - Imbalance-learn
  - TensorFlow)
- SQLite
- Tableau
- Google Slides
- Github



## Visualizations

To present our work we will utilize Tableau to create powerful visuals making our work, results, and analysis engaging and accessible.

- Import stock analysis data Data
- Connect Data
- Modify Data, rename and type
- Create Work Sheets
  - Class by sector
  - Earnings per Share
  - P Ratio
- Assemble Dashboard
- Add Written Analysis

Link to tableau story:
https://public.tableau.com/app/profile/samim.arif4259/viz/Finalprojectpresentation/FinalProjectPresentation?publish=yes
