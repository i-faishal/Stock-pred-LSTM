# Stock-pred-LSTM
PyTorch-based LSTM/GRU model for multi-output stock prediction using HCLTECH NIFTY-50 data. Uses 10-day input sequences of 11 features to predict next 5 days, evaluated with MSE, RMSE, MAE, and prediction graphs.

# Time Series Forecasting using LSTM (PyTorch)

## Features

* ✔ Data Cleaning (duplicate check, sorting by date)
* ✔ Date conversion to datetime format
* ✔ Handling missing values (forward fill, backward fill)
* ✔ Feature selection (11 stock features)
* ✔ Data normalization using l2 Normalizer
* ✔ Multi-output time-series forecasting
* ✔ LSTM model using PyTorch
* ✔ GPU support (CUDA if available)
* ✔ Model training with loss tracking
* ✔ Model evaluation using standard metrics

---

## Metrics Used

* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* Mean Absolute Error (MAE)

---

## Visualization

* Actual vs Predicted Close Price
* Helps compare model performance visually

---

## Dataset

* IOC Stock Data
* Total Records: 5306 rows

### Features Used:

* Prev Close
* Open
* High
* Low
* Last
* Close
* VWAP
* Volume
* Turnover
* Trades
* Deliverable Volume

---

## ML Pipeline

1. Load dataset (CSV)
2. Convert Date column to datetime
3. Sort data chronologically
4. Check & remove duplicates
5. Handle missing values
6. Normalize features
7. Create sequences

   * Input: last 10 days
   * Output: next 5 days
8. Train-test split (80-20)
9. Train LSTM model
10. Predict future values
11. Evaluate model performance
12. Plot predictions vs actual values

---

##  Model Details

* Model: LSTM (PyTorch)
* Input size: 11 features
* Hidden layers: 2
* Hidden size: 64
* Output: 5 future days × 11 features

---

## Tech Stack

* Python
* PyTorch
* Pandas
* NumPy
* Matplotlib
* Scikit-learn

---

## How to Run

```bash
# Clone repository
git clone <your-repo-link>

# Navigate to project folder
cd <your-folder>

# Install dependencies
pip install torch pandas numpy matplotlib scikit-learn

# Run notebook
jupyter notebook
```

---

## Results

* Model trained successfully on time-series data
* Predictions generated for next 5 days
* Evaluation metrics calculated
* Visualization shows close alignment between predicted and actual values

---

## Author

**Name:** MD Faishal

---
