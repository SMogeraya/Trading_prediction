# 📈 Fear & Greed Sentiment Impact on Trader Performance

## 🎯 Project Objective
The main goal of this project is to **analyze how market sentiment — particularly fear and greed — influences trader performance**, identify **hidden behavioral and performance patterns**, and **deliver insights that can drive smarter trading strategies**.

---

## 🧩 Overview
Market sentiment, measured through the **Fear and Greed Index**, often drives traders' emotions and decision-making.  
This project integrates **historical trading data** with **market sentiment scores** to study the correlation between **trader profits/losses** and the **overall mood of the market**.

By leveraging **data analysis, statistical testing, and machine learning**, we uncover how emotional extremes in the market affect trading outcomes and volatility.

---

## ⚙️ Key Features
- **Data Integration:** Merges historical trade data with the Fear & Greed Index dataset.  
- **Sentiment Categorization:** Classifies trading periods into *Extreme Fear, Fear, Neutral, Greed,* and *Extreme Greed*.  
- **Performance Analysis:** Visualizes and quantifies how trader PnL varies across sentiment categories.
- **Predictive Modeling:** Implements a Random Forest model to estimate trader PnL based on market sentiment and trade characteristics.  
- **Hidden Pattern Discovery:** Highlights volatility trends and risk exposure during emotional market phases.

---

## 🧠 Methodology
1. **Data Cleaning & Preprocessing**
   - Loaded `historical_data.csv` and `fear_greed_index.csv`
   - Merged datasets based on date/time
   - Converted trade sizes and prices to uniform scale

2. **Exploratory Data Analysis (EDA)**
   - Distribution plots of profit/loss by sentiment
   - Correlation heatmaps between numerical trading variables
   - Outlier and volatility pattern detection

3. **Machine Learning**
   - Random Forest Regression to predict profit/loss (`Closed_PnL`) based on:
     - Market Sentiment  
     - Trade Size  
     - Execution Price  
     - Trade Direction  
   - Evaluated with R² and MAE metrics

---

## 📊 Key Insights
- **Extreme market emotions (fear or greed)** lead to **higher volatility** — both large gains and losses are more common.  
- **Neutral sentiment periods** show **stable, low-risk** trading outcomes.  
- Average trader profit remains near zero across all sentiments, but **risk exposure** changes drastically.  
- Sentiment impacts **volatility and trade outcomes**, not guaranteed profit.

---

## 🧰 Technologies Used
| Category | Tools / Libraries |
|-----------|-------------------|
| Language | Python |
| Data Handling | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Statistics | SciPy |
| Machine Learning | Scikit-learn |
| Data Source | Fear & Greed Index, Historical Trader Data (CSV) |

---

## 📁 Dataset Information
### 1️⃣ `historical_data.csv`
| Column | Description |
|--------|--------------|
| Account | Trader ID |
| Coin | Cryptocurrency traded |
| Execution Price | Trade execution price |
| Size USD | Trade size in USD |
| Side | Buy/Sell direction |
| Closed PnL | Profit or loss from trade |
| Timestamp | Trade execution timestamp |

### 2️⃣ `fear_greed_index.csv`
| Column | Description |
|--------|--------------|
| Date | Date of recorded sentiment |
| FearGreedValue | Index score (0–100) |
| Sentiment | Label (Extreme Fear → Extreme Greed) |

---

## 📷 Visual Highlights
- Trader Profit/Loss Distribution across Market Sentiments  
- Correlation between Sentiment and PnL Volatility  
- Model Feature Importance (Random Forest)

---

## 🚀 How to Run
```bash
# 1️ Clone the repo
git clone https://github.com/your-username/fear-greed-trader-performance.git
cd fear-greed-trader-performance


# 2 Run the notebook or script
python analysis.py
