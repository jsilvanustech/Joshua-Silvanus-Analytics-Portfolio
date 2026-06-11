# From Volatility to Visibility: Forecasting High-Demand Gasoline Weeks Using Machine Learning

## Overview

This project was completed as part of a four-person machine learning consulting project in collaboration with Sunoco Supply & Trading. The objective was to develop a predictive model that could identify upcoming high-demand gasoline weeks while minimizing costly false positive alerts that could lead to unnecessary fuel allocation decisions.

Rather than optimizing purely for accuracy, our approach focused on aligning model performance with Sunoco's operational priorities by reducing incorrect high-demand signals.

---

## Business Problem

Gasoline demand is difficult to predict due to changes in economic conditions, transportation behavior, seasonality, fuel prices, and supply factors.

Incorrectly forecasting demand spikes can create operational inefficiencies, including unnecessary supply allocation and storage costs.

**Goal:** Create an early-warning system capable of identifying future high-demand weeks while limiting false alarms.

---

## My Contributions

As the primary technical contributor, my responsibilities included:

- Built the end-to-end machine learning pipeline from data preparation through final model evaluation
- Cleaned and transformed time-series datasets from multiple economic, transportation, weather, and energy sources
- Engineered predictive features including lag variables, percentage changes, and seasonal indicators to reflect real-world forecasting conditions
- Implemented and evaluated machine learning models including:
  - XGBoost
  - CatBoost
  - Neural Networks
- Designed a cost-sensitive evaluation framework prioritizing Sunoco's objective of minimizing false positives
- Tuned model thresholds to balance prediction accuracy with operational decision costs
- Developed model interpretation outputs including feature importance analysis
- Presented findings and business recommendations to Sunoco's supply chain team

---

## Methodology

### Feature Engineering

Created predictors from:

- Energy Supply:
  - Refinery utilization
  - Rig count

- Macroeconomic Indicators:
  - GDP
  - Unemployment
  - Economic indices

- Transportation Demand:
  - Vehicle miles traveled (VMT)
  - Automobile sales

- Market Conditions:
  - Gasoline prices
  - Crude oil prices

- Seasonality:
  - Heating degree days (HDD)
  - Cooling degree days (CDD)

Time-based lag features were created to ensure the model only used information available before the forecast period.

---

## Model Selection

Multiple models were evaluated:

| Model | Reason Evaluated |
|---|---|
| Neural Network | Ability to capture complex nonlinear patterns |
| CatBoost | Strong performance with structured datasets |
| XGBoost | Balance of predictive power, speed, and interpretability |

XGBoost was selected due to its strong performance on structured tabular data and ability to provide explainable feature insights.

---

## Results

Final Model Performance:

| Metric | Result |
|---|---:|
| High-demand weeks identified | 73% |
| Precision | 79% |
| True Positive / False Positive Ratio | 11:3 |
| False alerts | 3 annually |

The final model provided Sunoco with a reliable early-warning signal while limiting unnecessary operational responses.

---

## Key Insights

The strongest predictors of high-demand gasoline weeks were:

1. Time-based demand trends
2. Automobile sales patterns
3. Mobility indicators (Vehicle Miles Traveled)

These results highlighted how long-term consumer behavior and transportation patterns influence gasoline demand.

---

## Tools Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- CatBoost
- Matplotlib
- Jupyter Notebook

---

## Repository Contents

📁 notebook  
Complete machine learning workflow

📁 presentation  
Final stakeholder presentation
