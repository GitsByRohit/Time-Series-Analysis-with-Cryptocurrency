# 📊 Crypto Time Series Analysis & Decision Support Dashboard

An end-to-end **Time Series Analytics Dashboard** for cryptocurrencies, built using **Python & Streamlit**, focusing on **exploration, volatility analysis, forecasting, sentiment analysis, and executive decision support**.

This project analyzes **Bitcoin (BTC)** and **Ethereum (ETH)** using historical market data and NLP-based news sentiment to generate actionable insights.

---

## 🚀 Features

- 🔐 Secure Login & Signup (SQLite-based authentication)
- 📈 Exploratory Data Analysis (EDA)
- 📉 Volatility & Risk Analysis
- ⏳ Time Series Forecasting (ARIMA & Prophet)
- 🧠 NLP-based Sentiment Analysis (Google News RSS + VADER)
- 📌 Executive Insights & KPI Dashboard
- 🎨 Clean UI with custom CSS & Streamlit theming

---

## 🗂️ Project Structure
```
crypto-time-series-dashboard/
├── app.py
├── auth/
│   ├── auth.py
│   └── database.py
├── data/
│   ├── data_fetcher.py
│   ├── data_preprocessing.py
│   └── newsfetcher.py
├── analytics/
│   ├── eda.py
│   ├── volatility.py
│   ├── forecasting.py
│   ├── sentiment_analysis.py
│   └── insights.py
├── utils/
│   ├── config.py
│   ├── charts.py
│   └── helpers.py
├── assets/
│   └── styles.css
├── .streamlit/
│   └── config.toml
├── requirements.txt
├── .gitignore
└── README.md
```

### Explanation

- **app.py:** Main entry point (orchestration only)  
- **auth/:** Authentication & user management  
  - auth.py: Login & signup logic  
  - database.py: SQLite DB operations  
- **data/:** Data ingestion & preprocessing  
  - data_fetcher.py: Crypto price data fetching  
  - data_preprocessing.py: Cleaning & feature engineering  
  - newsfetcher.py: Google News RSS fetcher  
- **analytics/:** Analysis, forecasting & insights  
  - eda.py: Charts 1–8 (Exploratory Data Analysis)  
  - volatility.py: Charts 9–15 (Risk & volatility)  
  - forecasting.py: Charts 16–22 (Forecasting models)  
  - sentiment_analysis.py: NLP-based sentiment analysis  
  - insights.py: Charts 23–30 (Executive insights)  
- **utils/:** Shared utilities & helpers  
  - config.py: Constants & configuration  
  - charts.py: Common chart helpers  
  - helpers.py: Reusable helper functions  
- **assets/:** Static assets  
  - styles.css: Custom UI styling  
- **.streamlit/:** Streamlit configuration  
  - config.toml: Theme & app settings  
- **requirements.txt:** Project dependencies  
- **.gitignore:** Ignored files  
- **README.md:** Project documentation  



---

## 📊 Chart Deliverables Mapping (30 Charts)

### 📊 EDA (Charts 1–8)
- Price trends (BTC & ETH)
- Trading volume
- Market capitalization
- Daily & log returns
- Price distribution

### 📉 Volatility & Risk (Charts 9–15)
- Rolling volatility
- Bollinger Bands (BTC & ETH)
- High–low spread
- Risk vs return
- Returns boxplot

### ⏳ Forecasting (Charts 16–22)
- Trend, seasonality, residuals
- ARIMA forecast
- Prophet forecast
- Actual vs predicted
- Confidence intervals

### 📌 Insights & KPIs (Charts 23–30)
- Best & worst performer
- Monthly returns heatmap
- Moving average crossover
- Buy/Sell signals
- ROI, volatility, drawdown
- Correlation matrix
- Executive summary dashboard

---

## 🧠 Sentiment Analysis

- Source: **Google News RSS**
- NLP Model: **VADER Sentiment Analyzer**
- Analyzes crypto-related news headlines
- Outputs sentiment scores & polarity trends
- Integrated into dashboard as a dedicated module

---

## 👥 Team Role Distribution

| Teammate | Responsibility |
|--------|----------------|
| Authentication Lead | Login, signup, DB, session handling |
| EDA Analyst | Market exploration & EDA charts |
| Volatility Analyst | Risk & volatility modeling |
| Forecasting Specialist | Time series forecasting |
| Insights Lead | KPIs, summaries, decision support |

---

## ⚙️ Installation & Run Instructions

### 1️⃣ Create virtual environment
```bash
python -m venv venv
venv\Scripts\activate   # Windows
```
2️⃣ Install dependencies
```
pip install -r requirements.txt
```
3️⃣ Download sentiment lexicon (one-time)
```
python -m nltk.downloader vader_lexicon
```

4️⃣ Run the app
```
streamlit run app.py
```

## 📌 Conclusion

This dashboard provides a comprehensive analytical framework for understanding cryptocurrency markets by combining statistical analysis, forecasting, and sentiment intelligence into a single decision-support platform.
