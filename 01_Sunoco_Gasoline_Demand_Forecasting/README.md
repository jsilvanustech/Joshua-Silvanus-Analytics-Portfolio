# Predicting High-Demand Gasoline Weeks Using Machine Learning


## Business Problem

Gasoline demand volatility creates challenges for fuel supply planning.
Incorrectly predicting demand spikes can lead to unnecessary storage 
and allocation costs.

The objective was to build a predictive system that identifies upcoming
high-demand weeks while minimizing costly false positives.


## Solution

Created an XGBoost classification model using:

- Energy production indicators
- Macroeconomic variables
- Transportation and mobility trends
- Fuel price indicators
- Weather seasonality factors


## Machine Learning Approach

- Feature engineering with lagged indicators
- Time-aware train/test validation
- Model comparison:
    - Neural Networks
    - CatBoost
    - XGBoost
- Cost-sensitive threshold optimization


## Results

| Metric | Result |
|---|---:|
| High Demand Weeks Identified | 73% |
| Precision | 79% |
| True Positive : False Positive Ratio | 11:3 |
| False Alarms | 3/year |


## Business Impact

Created an early-warning signal allowing supply teams to better anticipate
demand spikes and reduce unnecessary operational costs.


## Tools

Python  
Pandas  
Scikit-Learn  
XGBoost  
Matplotlib
