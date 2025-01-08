# Time Series Forecasting 

 ## Time Series Analysis and Forecasting of Airline Passenger Data

This project demonstrates time series analysis and forecasting using airline passenger data. The objective is to analyze monthly passenger counts, check the stationarity of the time series, and build an ARIMA model for future forecasting.


## Project Overview
The project involves performing exploratory data analysis (EDA) on the airline passenger dataset, checking the stationarity of the data, and applying ARIMA modeling to forecast passenger counts for future months.

## Dataset
The dataset used in this project is `AirPassengers.csv`, which contains:
- **Month**: The month of observation.
- **#Passengers**: The number of airline passengers for that month.

## Methodology
1. **Loading and Exploring the Data**:
   - The dataset is loaded using Pandas, and initial exploration includes checking for missing values, data types, and summary statistics.

2. **Data Visualization**:
   - A time series plot of monthly passenger counts is created to observe trends and seasonality.

    ![image](https://github.com/user-attachments/assets/aa38d391-f0bc-4248-a7ad-95816d700452)


3. **Stationarity Check**:
   - The Augmented Dickey-Fuller (ADF) test is used to check if the time series is stationary.

4. **ARIMA Modeling**:
   - The best ARIMA model parameters are selected using Pmdarima's `auto_arima` function.
   - The selected ARIMA model is fitted, and in-sample predictions are generated.
  
    ![image](https://github.com/user-attachments/assets/b94cfe93-2cf7-4986-a6a7-5de7e932b9b8)


5. **Forecasting**:
   - The fitted ARIMA model is used to forecast passenger counts for the next 24 months.
  
  ![image](https://github.com/user-attachments/assets/4e7e1aea-8797-4f7e-935f-6a5e50db3c3e)




## Dependencies
The project requires the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `statsmodels`
- `pmdarima`

To install the dependencies, run:
```bash
pip install pandas numpy matplotlib statsmodels pmdarima
```

## How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/airline-passenger-forecast.git
   ```
2. Navigate to the project directory:
   ```bash
   cd airline-passenger-forecast
   ```
3. Ensure all dependencies are installed.
4. Run the Jupyter notebook `project.ipynb` to reproduce the analysis and results.



