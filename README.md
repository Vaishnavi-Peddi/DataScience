
# 📊 Trader Behavior vs Market Sentiment Analysis
**Data Science Assignment – Web3 Trading Team**

## 📌 Project Overview
This project analyzes how trader behavior varies under different Bitcoin market sentiment regimes such as **Fear, Greed, Extreme Greed, and Neutral**.
The objective is to understand how **profitability, trading activity, and buy/sell behavior** align with market sentiment and to derive insights for smarter trading strategies.

## 📂 Project Structure
```
ds_vaishu/
│
├── notebook_1.ipynb        # Google Colab notebook with full analysis
├── csv_files/              # Raw and processed CSV datasets
│   └── merged_trader_sentiment_data.csv
│
├── outputs/                # Visualizations and plots
│   └── *.png
│
├── ds_report.pdf           # Final summarized insights and conclusions
└── README.md               # Project documentation
```

## 📊 Datasets Used

### 1️⃣ Bitcoin Market Sentiment Dataset
- Columns:
  - Date
  - Classification (Fear / Greed / Extreme Greed / Neutral)

### 2️⃣ Historical Trader Data (Hyperliquid)
- Key Columns:
  - account
  - symbol
  - time
  - side (buy/sell)
  - size
  - closedPnL
  - leverage

## ⚙️ Methodology
1. Data loading and initial exploration  
2. Timestamp conversion (Unix → Date & Time)  
3. Data cleaning and normalization  
4. Merging trader data with sentiment data  
5. Feature engineering (PnL flags, risk levels)  
6. Exploratory Data Analysis and visualization  

## 📈 Key Insights
- Fear sentiment shows the highest trading activity, indicating panic-driven behavior.
- Large PnL outliers occur mostly during Fear periods.
- Greed periods exhibit more confident but controlled trading.
- Selling pressure increases during Fear sentiment.
- Market sentiment strongly influences trader risk appetite.

## 💡 Trading Implications
- Sentiment can be used as a risk-adjustment signal.
- Reduce leverage and position sizes during Fear.
- Apply disciplined risk management during Greed to avoid overconfidence.

## ▶️ How to Run
1. Open `notebook_1.ipynb` in Google Colab.
2. Upload the required CSV files.
3. Run all cells sequentially.
4. Review visualizations and insights.
5. Refer to `ds_report.pdf` for conclusions.

## 🧠 Conclusion
This project demonstrates that trader behavior is highly sentiment-driven. Incorporating sentiment-aware signals into trading strategies can improve consistency, reduce emotional bias, and enhance risk management.
