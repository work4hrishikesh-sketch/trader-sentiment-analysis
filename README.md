# Trader Performance vs Market Sentiment

## Objective
The goal of this project is to analyze how market sentiment (Fear vs Greed)
impacts trader behavior and performance on the Hyperliquid platform.
The analysis aims to uncover patterns that can help inform better trading
decisions under different market conditions.

---

## Datasets Used
1. **Bitcoin Fear & Greed Index**
   - Daily market sentiment classified as Fear or Greed

2. **Historical Trader Data (Hyperliquid)**
   - Trade-level data including account, trade size, direction, timestamps,
     and closed PnL

---

## Methodology

### 1. Data Preparation
- Loaded and inspected both datasets
- Checked for missing values and duplicates
- Normalized column names for consistency
- Converted millisecond timestamps to datetime
- Aligned both datasets on a daily level using date

### 2. Feature Engineering
Created daily trader-level metrics:
- Daily PnL
- Number of trades per day
- Average trade size
- Win rate
- Long/short bias

### 3. Analysis
- Compared trader performance on Fear vs Greed days
- Analyzed behavioral changes such as trade frequency and directional bias
- Segmented traders into:
  - Frequent vs Infrequent traders
  - Consistent vs Inconsistent traders

---

## Key Insights
- Trader performance differs across Fear and Greed market conditions
- Greed periods generally show higher profitability but increased volatility
- Frequent traders are more sensitive to market sentiment
- Consistent traders maintain relatively stable win rates across conditions

---

## Strategy Suggestions
- During Fear days, highly risky or frequent traders should reduce trading
  activity to limit potential drawdowns.
- During Greed days, increased trading activity should be allowed only for
  consistent traders who show stable performance.

---

## Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

---

## How to Run
1. Clone or download the repository
2. Open the notebook in Jupyter Notebook
3. Run cells in order to reproduce the analysis
