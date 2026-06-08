# Bitcoin Market Sentiment vs Trader Performance Analysis

## Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance using Hyperliquid historical trading data and the Bitcoin Fear & Greed Index.

The objective is to identify how market sentiment influences trader profitability, trading behavior, and overall performance. By combining market sentiment data with real trading activity, the analysis aims to uncover actionable insights that can support better trading and risk-management decisions.

---

## Datasets Used

### 1. Bitcoin Fear & Greed Index Dataset

Columns:

* date
* value
* classification

This dataset provides daily Bitcoin market sentiment categorized into:

* Extreme Fear
* Fear
* Neutral
* Greed
* Extreme Greed

### 2. Hyperliquid Historical Trader Data

Columns include:

* Account
* Coin
* Execution Price
* Size Tokens
* Size USD
* Side
* Timestamp IST
* Direction
* Closed PnL
* Fee
* Trade ID

This dataset contains historical trading records and trader performance metrics.

---

## Methodology

### Data Cleaning

* Loaded both datasets using Pandas.
* Converted timestamp fields into datetime format.
* Extracted date values from trading timestamps.
* Checked for missing values and data consistency.

### Data Integration

* Merged the trading dataset with the Fear & Greed Index dataset using the date column.
* Assigned a sentiment label to each trade.

### Exploratory Data Analysis

The following analyses were performed:

1. Sentiment Distribution Analysis
2. Average PnL by Sentiment
3. Total Profit by Sentiment
4. Win Rate Analysis
5. Buy vs Sell Behavior
6. Long vs Short Position Analysis
7. Top Trader Performance
8. Coin-wise Profitability Analysis
9. PnL Distribution Analysis
10. Correlation Analysis

---

## Tools and Libraries

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Key Findings

* Fear and Greed periods accounted for the majority of trading activity.
* Trader profitability varied significantly across sentiment categories.
* Positive market sentiment generally corresponded with improved trading performance.
* Long positions were more common during Greed and Extreme Greed periods.
* Extreme Fear periods showed relatively weaker trading outcomes.

---

## Business Recommendations

1. Incorporate market sentiment indicators into trading strategies.
2. Reduce leverage exposure during Extreme Fear periods.
3. Use sentiment changes as an additional risk-management signal.
4. Combine sentiment indicators with technical analysis for stronger decision-making.
5. Integrate sentiment features into algorithmic trading models.

---

## Conclusion

This analysis demonstrates that Bitcoin market sentiment has a measurable impact on trader behavior and performance. By combining sentiment indicators with historical trading data, traders and trading platforms can gain valuable insights into market conditions and improve risk-adjusted decision-making.

The results highlight the importance of sentiment-aware trading strategies and provide a foundation for further predictive modeling and advanced quantitative research.
