

📊 Market Sentiment vs Trader Performance – ML Analysis

This project explores the relationship between Bitcoin market sentiment and trader performance using a combination of historical trade data and Fear & Greed Index sentiment data. It applies data analysis and machine learning to uncover insights and build a predictive model for trade profitability.

🔍 Project Overview

Analyze trader behavior under varying market sentiments (Fear vs Greed).

Investigate how sentiment affects trade size, PnL, direction (buy/sell), and profitability.

Build a machine learning model to predict whether a trade will be profitable based on trade features and sentiment indicators.

📁 Dataset
1. Bitcoin Market Sentiment Dataset

Source: Fear & Greed Index

Columns:

date: YYYY-MM-DD

value: Integer sentiment score (0-100)

classification: e.g., "Fear", "Greed", "Extreme Fear"

2. Hyperliquid Trader History Dataset

Columns:

timestamp_ist, side, size_usd, closed_pnl, coin, etc.

Contains 210,000+ individual trades across multiple accounts.

📌 Both datasets are merged on the date column for analysis.
🧪 Project Pipeline

Data Cleaning & Preprocessing

Parsed timestamps

Extracted date for merging

Encoded categorical variables (side, coin, classification)

Added derived columns: profitable (PnL > 0)

EDA (Exploratory Data Analysis)

Profitability by sentiment class

Trade direction vs sentiment

Average trade size and PnL by sentiment

Distribution plots and trends over time

Machine Learning

Task: Binary classification → Predict if a trade is profitable

Features:

Sentiment score (value)

Sentiment class (classification)

Trade size, fee, direction, coin

Model: Random Forest Classifier

Evaluation: Accuracy, classification report
📈 Key Findings

Trades during "Fear" periods had slightly higher profitability on average.

"Sell" trades during fearful markets performed better than "Buy" trades.

Sentiment score has weak correlation with profitability, but adds predictive power when combined with other features.

Random Forest model achieved ~X% accuracy (you can fill in the real number).
📌 View the full model and visualizations in the notebook.
