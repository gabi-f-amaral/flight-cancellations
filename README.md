# Flight Cancellation Prediction in Australia

## Project Overview
This project predicts the probability of flight cancellations on Australian domestic routes using historical flight data from 2010 to 2025.

The objective is to allow users to ask:
> "What is the probability that my flight will be cancelled on a given route and month in 2026?"

## Data
- Source: Australian domestic flight statistics
- Granularity: Route × Month (all airlines)
- Period: January 2010 – August 2025
- Pandemic period (2020–2023) excluded from modeling

## Methodology
- Data cleaning and aggregation
- Exploratory data analysis
- Feature engineering (lags, seasonality)
- Binary classification models (Logistic Regression, Random Forest, Gradient Boosting)
- Model evaluation using F1-score and PR-AUC
- Forecasting cancellation risk for 2026

## Repository Structure
flight-cancellation-prediction/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── data/
│   ├── raw/
│   │   └── flights_raw.csv
│   ├── processed/
│   │   └── flights_cleaned.csv
│
├── notebooks/
│   ├── 01_data_loading_and_quality.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_feature_engineering.ipynb
│   ├── 04_modeling.ipynb
│   └── 05_forecasting_2026.ipynb
│
├── src/
│   ├── __init__.py
│   ├── data_cleaning.py
│   ├── feature_engineering.py
│   ├── modeling.py
│   ├── evaluation.py
│   └── utils.py
│
├── reports/
│   ├── data_quality_report.md
│   ├── figures/
│   └── final_presentation.pptx
│
├── models/
│   └── best_model.pkl
│
└── app/
    ├── app.py          # future web app / Streamlit
    └── chatbot.py      # future LLM logic

## Results
(placeholder for later)

## Future Work
- Web dashboard
- Interactive map
- LLM-powered chatbot
