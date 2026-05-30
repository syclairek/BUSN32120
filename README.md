# News Sentiment and Market Reaction Analysis

## Overview
This project analyzes the relationship between financial news sentiment and S&P 500 market behavior using SQL, Python, NLP, and machine learning techniques.

We investigate whether news sentiment can help explain or predict short-term market returns, volatility, and broader market conditions.

The project combines:
- SQL-based feature engineering
- Exploratory data analysis (EDA)
- Sentiment analysis
- Predictive modeling
- Market volatility analysis

---

## Research Question

Can financial news sentiment predict market reactions?

More specifically:
- Does positive or negative sentiment affect daily market returns?
- Do lagged or rolling sentiment measures improve predictive power?
- Is news volume more closely related to market volatility than return direction?

---

## Datasets

### 1. Financial News Sentiment Dataset
Contains:
- News publication dates
- Sentiment scores
- Sentiment labels
- News volume information

### 2. S&P 500 Market Data
Contains:
- Daily returns
- Lagged returns
- Market volatility measures

---

## Technologies Used

### SQL
- Joins
- Window functions
- Grouping and aggregation
- Rolling calculations
- Feature engineering

### Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

### Models
- Linear Regression
- Logistic Regression
- K-Means Clustering

---

## Feature Engineering

To better capture market behavior, several engineered features were created:

- Lagged sentiment
- 3-day rolling sentiment
- Absolute returns (volatility proxy)
- News volume groups
- Sentiment-volume interaction features
- Volatility ranking

---

## Key Findings

### 1. Sentiment alone showed limited predictive power
Linear and logistic regression models showed weak ability to predict short-term market direction.

### 2. Rolling sentiment was more informative than raw daily sentiment
Temporal sentiment features provided slightly clearer patterns than isolated daily sentiment scores.

### 3. News volume was more strongly related to volatility than returns
Periods with heavier news activity tended to exhibit larger absolute market movements.

### 4. Market behavior appeared highly context-dependent
The relationship between sentiment and returns varied depending on broader market conditions and news intensity.

---

## Modeling Results

| Model | Key Result |
|---|---|
| Linear Regression | Near-zero explanatory power (R² ≈ 0) |
| Logistic Regression | ~54.7% accuracy |
| K-Means Clustering | Identified distinct market regimes |

---

## Project Structure

```bash
├── data/
├── sql/
│   └── SQL_Based_Extended_Sentiment_Analysis.ipynb
├── notebooks/
│   └── news_sentiment_final.ipynb
├── presentation/
│   └── Financial_News_Sentiment.pdf
├── README.md