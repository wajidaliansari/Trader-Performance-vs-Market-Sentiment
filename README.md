## Trader-Performance-vs-Market-Sentiment
   A data analysis project exploring the relationship between trader performance and market sentiment with insights and recommendations.
   Market Sentiment vs Trader Behavior Analysis

##Project Overview
   This project analyzes how **market sentiment (Fear vs Greed)** impacts **trader behavior and performance** using Bitcoin sentiment data and Hyperliquid trading data.

   The goal is to uncover patterns that can help in building smarter trading strategies.



 ## Datasets Used

###  Bitcoin Market Sentiment Dataset
- Columns:
  - Date
  - Classification (Fear / Greed)

### Historical Trader Data (Hyperliquid)
- Key Features:
  - account
  - symbol
  - execution price
  - size
  - side (LONG / SHORT)
  - time
  - closedPnl
  - leverage

---

##  Steps Performed

###  Data Cleaning
- Removed missing values
- Removed duplicate records
- Converted timestamps into proper datetime format

###  Data Transformation
- Converted data to **daily level**
- Aligned both datasets using date

###  Feature Engineering
Created important trading metrics:
- Daily Profit & Loss (PnL)
- Number of trades per day
- Average trade size
- Win rate (profitable trades)
- Average leverage
- Long/Short ratio

###  Data Merging
- Merged sentiment dataset with trading metrics using date

---

##  Analysis & Visualization

The following relationships were analyzed:

-  PnL vs Sentiment (Fear vs Greed)
-  Number of trades vs Sentiment
-  Win rate vs Sentiment
-  Leverage usage vs Sentiment
-  Correlation between all features

---

##  Key Insights

- Traders tend to **trade more during Greed periods**
- **Leverage is higher during Greed**, indicating riskier behavior
- **Win rate may be higher during Fear**, suggesting cautious trading
- Market sentiment strongly influences trading decisions and outcomes

---

##  Machine Learning (Optional)
A simple **Linear Regression model** was used to predict PnL based on:
- Number of trades
- Average trade size
- Leverage
- Long/Short ratio

---

##  Tech Stack

- Python 
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---


