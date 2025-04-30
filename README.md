# LSTM_model-_for_time-series_forecasting

# Air Passengers Time Series Forecasting with LSTM

## Overview

This repository demonstrates how to forecast the monthly number of international airline passengers using the classic [AirPassengers](AirPassengers.csv) dataset and a Long Short-Term Memory (LSTM) neural network. The LSTM model is implemented in Python and predicts future passenger counts based on historical data.

## Dataset

- **File:** `AirPassengers.csv`
- **Columns:**
    - `Month`: Date in YYYY-MM format
    - `#Passengers`: Number of passengers for that month

Example (last row in the dataset):


| Month | \#Passengers |
| :-- | :-- |
| 1960-12 | 432 |

## How It Works

1. **Data Preprocessing**
    - The dataset is loaded and the `Month` column is converted to datetime.
    - The passenger numbers are normalized for stable model training.
    - Input sequences are created using a sliding window (e.g., the previous 12 months to predict the next month).
2. **LSTM Model**
    - A Long Short-Term Memory (LSTM) neural network is used for time series forecasting.
    - The model learns patterns such as trend and seasonality from the historical data.
3. **Training and Evaluation**
    - The model is trained on the historical data.
    - After training, the model predicts passenger numbers for future months.
    - The results are visualized by plotting the actual vs. predicted passenger numbers.

## How to Run

1. **Clone the repository and navigate to the project folder:**

```bash
git clone https://github.com/prodigalson6770/LSTM_model_for_timeseries_forecasting
cd LSTM_model_for_time-series_forecasting
```

2. **Ensure you have the required dependencies:**
    - Python 3.x
    - numpy
    - pandas
    - matplotlib

Install with:

```bash
pip install numpy pandas matplotlib 
```

3. **Place the `AirPassengers.csv` file in the project directory.**
4. **Run the notebook or Python script:**
    - For Jupyter Notebook, open and run all cells.
    - For a Python script, run:

```bash
python LSTM_Forecasting_Model.py
```

5. **View the Results:**
    - The script will display a plot comparing the actual and predicted passenger numbers.
    - Training loss and model accuracy are also printed.

## Example Output

- **Actual vs Predicted Plot:**
The script generates a graph showing how closely the model’s predictions match the actual passenger numbers.
- **Sample Output:**

```
Epochs : 500
Model prediction accuracy: 92.80%
```


## References

- [AirPassengers Dataset](https://datamarket.com/data/set/22u3/airline-passenger-miles-usa-1937-1960)
- [LSTM for Time Series Forecasting – Machine Learning Mastery](https://www.machinelearningmastery.com/time-series-prediction-lstm-recurrent-neural-networks-python-keras/)

---

**Feel free to fork, modify, and experiment with the model and dataset! For any questions or issues, please open an issue on this repository.**



