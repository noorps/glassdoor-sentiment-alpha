# Glassdoor Alpha: Corporate Culture as a Market Indicator

![Correlation Chart](correlation_chart.png)

## Project Overview
This project investigates the hypothesis that **Information Asymmetry** exists between a company's employees and the public equity markets. By analyzing historical employee reviews, we aim to determine if internal sentiment regarding "Senior Management" acts as a leading indicator for stock price performance.

## Methodology
* **Data Sources:**
    * **Alternative Data:** Historical Glassdoor reviews (2008-2019) focusing on "Senior Management" star ratings.
    * **Market Data:** Historical OHLCV stock data via the Yahoo Finance API.
    * **Technique:**
    * Natural Language Processing (NLP) for sentiment extraction (VADER).
    * Time-series alignment using monthly rolling averages to smooth volatility.
    * Dual-axis visualization to identify divergence signals.

## Key Findings
* **Correlation:** Observed a positive correlation coefficient of about **0.30**, suggesting a moderate link between employee confidence and shareholder value.
* **Lag Effect:** Visual analysis suggests that declines in management ratings often precede stock price corrections, validating the potential of this signal for risk management models.

## Technologies Used
* Python (Pandas, NumPy)
* Scikit-Learn (Random Forest)
* Matplotlib / Seaborn
* Yahoo Finance API (`yfinance`)

## How to Run
1.  Open the notebook in Google Colab.
2.  Upload the `glassdoor_reviews.csv` dataset.
3.  Run the pipeline to reproduce the visualization.
