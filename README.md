## 📊 Trader Behavior vs Bitcoin Market Sentiment

### 🧠 Objective

This project explores the relationship between **trader performance** and **Bitcoin market sentiment** (Fear vs. Greed), using historical trade execution data and sentiment index. The goal is to uncover actionable insights and suggest smarter trading strategies based on behavioral patterns.

---

### 📁 Datasets

1. **Bitcoin Market Sentiment Dataset**

   * Columns: `date`, `classification` (Fear/Greed)
   * Source: Alternative.me Fear-Greed Index

2. **Historical Trader Data (Hyperliquid)**

   * Columns: `Account`, `Coin`, `Execution Price`, `Size USD`, `Closed PnL`, `Timestamp IST`, etc.

---

### 🔧 Tools Used

* **Python 3.10+**
* **Pandas**
* **Seaborn & Matplotlib** for visualization
* **Jupyter Notebook / Google Colab**

---

### 🔍 Process Overview

#### 1. Data Cleaning & Preparation

* Parsed timestamps from both datasets
* Merged sentiment data into trader data using date alignment
* Cleaned and converted `Closed PnL` values

#### 2. Exploratory Data Analysis

* **PnL Summary by Sentiment** (Mean, Median, Count)
* **Win Rate Analysis** (% of profitable trades per sentiment)
* **Top Trader Analysis** (Best performing accounts under Fear vs Greed)

#### 3. Visualization

* Bar plots for average `Closed PnL` and win rate under each sentiment category

---

### 📈 Key Findings

| Metric          | Fear     | Greed      |
| --------------- | -------- | ---------- |
| Avg. PnL        | Lower    | Higher     |
| Win Rate        | Lower    | Higher     |
| Trader Behavior | Cautious | Aggressive |

> Detailed numbers available in the notebook and output tables.

---

### 💡 Insights & Recommendations

* **Greed periods** lead to significantly higher profitability and success rates.
* **Fear periods** show more cautious trader behavior and inconsistent outcomes.
* Top traders are more active and successful during **Greed**, indicating strong momentum-based strategies.

#### ✅ Suggested Actions:

* Build trading bots or alerts that capitalize on “Greed” periods.
* Reduce exposure or automate defensive strategies during “Fear”.
* Monitor and model top-performing accounts for strategic replication.
