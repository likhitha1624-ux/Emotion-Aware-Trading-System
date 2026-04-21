# Emotion-Aware-Trading-System

Project Overview
Emotion-Aware Trading System that analyzes the relationship between Bitcoin market sentiment (Fear/Greed) and trader performance to generate smart trading strategies.

Objective
To understand how market emotions influence trading behavior and profitability, and to build a simple strategy system based on sentiment.


Datasets Used

1. Bitcoin Market Sentiment Dataset (Fear/Greed Index)
2. Historical Trader Data (Hyperliquid)



 Steps Performed

 1. Data Loading

* Imported both datasets using Pandas
* Loaded CSV files into DataFrames

2. Data Cleaning

* Checked missing values
* Removed null values using `dropna()`
* Ensured data consistency

3. Date Conversion

* Converted date columns into proper datetime format
* Created a common `Date` column for merging

4. Data Merging

* Merged sentiment and trader datasets using the Date column
* Combined market emotion with trading activity

 5. Feature Engineering

* Converted sentiment into numerical values (Fear = -1, Greed = 1)
* Created new columns:

  * Sentiment Score
  * Strategy (BUY / SELL / HOLD)
  * Profit indicator

 6. Strategy Development

* Built an emotion-based trading logic:

  * Fear + Profit → BUY
  * Greed + Loss → SELL
  * Otherwise → HOLD

7. Data Analysis

* Analyzed profit based on sentiment
* Compared win rate (profit vs loss)
* Studied trader behavior patterns

 8. Visualization

 Created bar charts for:

  * Profit vs Sentiment
  * Strategy performance
  * Win rate
* Used pie chart for trading activity

#9. Result Generation

* Generated insights on trader performance
* Exported final dataset


 Key Insights

* Trader performance varies with market sentiment
* Fear markets show controlled trading behavior
* Greed markets lead to aggressive trading
* Sentiment-based strategies improve decision-making

Tools Used

* Python
* Pandas
* Matplotlib

Conclusion

Market sentiment plays a major role in trading decisions.
Combining sentiment data with trading activity helps in building smarter strategies.




