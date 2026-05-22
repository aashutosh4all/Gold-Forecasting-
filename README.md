# Gold Price Forecasting & News Risk Dashboard

This project forecasts 7-day future gold prices using a return-based LSTM model and combines the forecast with live macro-news sentiment analysis.

## Features

- 7-day gold price forecasting using LSTM
- Historical gold futures price trend visualization
- Naive baseline comparison
- Live gold-related news fetching using Tavily
- News sentiment and risk analysis using Groq
- Combined model + news-based recommendation
- Streamlit dashboard

## Final Model

The final selected model is a Gold Market-Only Return-Based LSTM.

It outperformed the naive baseline:

| Model | MAE | RMSE | MAPE | R2 |
|---|---:|---:|---:|---:|
| Naive Baseline | 167.19 | 217.40 | 3.75 | 0.786 |
| Gold Return-Based LSTM | 160.79 | 213.36 | 3.60 | 0.794 |

## Tech Stack

Python, TensorFlow, Streamlit, Plotly, yFinance, Tavily API, Groq API

## Disclaimer
This project is for educational and analytical purposes only. It is not financial advice.

## How to Run

```bash
pip install -r requirements.txt
streamlit run app.py

