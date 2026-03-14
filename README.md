# Trader Behavior vs Market Sentiment Analysis

## Overview

This project analyzes how **Bitcoin market sentiment (Fear vs Greed)** influences **trader behavior and performance** on the Hyperliquid trading platform.

By combining **market sentiment data** with **historical trading activity**, the analysis explores whether trader profitability, trading frequency, and position bias change during different market conditions.

The goal is to uncover insights that could help design **smarter trading strategies based on sentiment signals**.

---

# Dataset

Two datasets were used in this analysis:

### 1. Bitcoin Fear & Greed Index

Contains daily sentiment classification of the crypto market.

Columns:

* `timestamp`
* `value`
* `classification` (Fear, Extreme Fear, Greed, etc.)

### 2. Historical Trader Data (Hyperliquid)

Contains trade-level information about traders.

Important columns:

* `Account` – trader identifier
* `Coin` – traded asset
* `Execution Price` – trade price
* `Size USD` – trade size
* `Side` – buy/sell direction
* `Timestamp` – trade execution time
* `Closed PnL` – profit or loss from trade

---

# Project Structure

```
project/
│
├── trader_analysis.ipynb
├── fear_greed_index.csv
├── historical_data.csv
├── images/
│   ├── performance_by_sentiment.png
│   ├── behavior_by_sentiment.png
│   ├── segmentation_pnl.png
│   └── consistency_analysis.png
└── README.md
```

---

# Setup

Install the required Python libraries.

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

# How to Run

1. Clone the repository

```
git clone https://github.com/your-username/trader-sentiment-analysis.git
cd trader-sentiment-analysis
```

2. Ensure the datasets are in the project folder:

* `fear_greed_index.csv`
* `historical_data.csv`

3. Run the analysis notebook

```
jupyter notebook analysis.ipynb
```

The notebook performs:

* Data preprocessing
* Dataset merging
* Feature engineering
* Trader segmentation
* Visualization and insights

---

# Methodology

The analysis follows these steps:

### 1. Data Preparation

* Loaded sentiment and trading datasets
* Cleaned column names and handled duplicates
* Converted timestamps to daily dates
* Merged datasets on date

### 2. Feature Engineering

Key metrics were computed:

* Daily PnL per trader
* Win rate
* Average trade size
* Number of trades per day
* Long/Short trading ratio

### 3. Trader Segmentation

Traders were segmented based on:

* Trading frequency (Frequent vs Infrequent)
* Profit consistency
* Trading direction bias

### 4. Visualization

Multiple charts were created to analyze:

* Performance differences between Fear and Greed periods
* Changes in trading activity
* Behavioral differences across trader segments

---

# Key Insights

### 1. Sentiment Influences Trader Performance

Traders tend to achieve higher average profits during **Greed periods**, while **Fear periods** show lower win rates and more volatile performance.

### 2. Trading Activity Increases During Greed

Greed sentiment correlates with higher trade frequency and larger average trade sizes, indicating increased market participation.

### 3. Frequent Traders Show Higher Returns but Higher Risk

Frequent traders often generate higher profits but experience greater variability in performance compared to infrequent traders.

---

# Strategy Recommendations

### Strategy 1 — Reduce Risk During Fear Markets

During Fear sentiment periods:

* Lower trade size
* Reduce leverage
* Focus on fewer high-confidence trades

### Strategy 2 — Increase Participation During Greed Markets

During Greed sentiment periods:

* Traders may increase trade frequency
* Momentum-based strategies may perform better
* Maintain proper risk management

---

# Conclusion

This analysis demonstrates that **market sentiment significantly influences trader behavior and profitability**. Incorporating sentiment indicators into trading strategies could help traders adjust risk exposure and improve decision-making.

---

# Author

Rohan Kumar P S
Data Analyst / Data Science Enthusiast
# trader-sentiment-analysis
Analysis of trader performance vs. market sentiment (Fear/Greed) on Hyperliquid. Includes data alignment, behavioral segmentation, and actionable trading strategies for the Primetrade.ai Data Science assignment.
