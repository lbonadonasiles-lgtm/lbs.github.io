# Energy Demand Forecasting

Predicting household electricity consumption using machine learning and time-series analysis.

## Overview

This project builds a machine learning pipeline to forecast energy demand using the [UCI Individual Household Electric Power Consumption](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption) dataset. The dataset contains approximately 2 million minute-by-minute readings of electricity usage from a single household over 4 years (2006–2010).

The goal is to predict **Global Active Power** (total household energy consumption in kilowatts) using time-based features and historical usage patterns.

## Key Findings

- **Seasonal patterns:** Energy consumption peaks during winter months (November–February), driven primarily by heating demand.
- **Daily patterns:** Usage is highest between 7–10 PM when occupants are home, lights are on, and appliances are running. Lowest usage occurs between 2–5 AM.
- **Lag features dramatically improved model performance**, confirming that recent usage history is the strongest predictor of future demand.

## Model Comparison

Three models were trained and evaluated:

| Model | R² (Before Lag Features) | R² (After Lag Features) |
|---|---|---|
| Linear Regression | 0.10 | 0.53 |
| Random Forest | 0.19 | 0.59 |
| **XGBoost** | **0.30** | **0.61** |

XGBoost achieved the best performance with an R² of 0.61 after feature engineering.

## Features Used

**Time-based features:** hour, day of week, month, day of year, week of year, weekend indicator

**Lag features:** usage 1 hour ago, 2 hours ago, 24 hours ago (same hour yesterday), 168 hours ago (same hour last week), and a 24-hour rolling average

## Tools & Libraries

- **Python** — programming language
- **Pandas** — data loading and manipulation
- **NumPy** — numerical computations
- **Matplotlib & Seaborn** — data visualization
- **Scikit-learn** — Linear Regression, Random Forest, evaluation metrics
- **XGBoost** — gradient boosting model
- **Jupyter Notebook** — development environment

## How to Run

1. Download the dataset from [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption)
2. Place the file in your Downloads folder
3. Open `energydemand.ipynb` in Jupyter Notebook (Anaconda)
4. Run the cells in order from top to bottom

## Limitations

The model captures approximately 61% of the variance in energy demand. The remaining 39% is likely influenced by factors not present in the dataset, such as outdoor temperature, weather conditions, holidays, and occupancy patterns. Adding external weather data would likely improve performance.

## Author

**Luciano Bonadona Siles**
- B.S. Biomedical Engineering, Minor in Computer Science — University of Arkansas
- [LinkedIn](https://www.linkedin.com/in/luciano-bonadona-2b39b3304/)
- l.bonadonasiles@gmail.com
