
# Gold Price Prediction  

## Overview  
This project predicts **gold prices** using machine learning, specifically a **Random Forest Regressor**. The dataset includes financial indicators such as stock indices, oil prices, silver prices, and exchange rates.  

## Dataset  
The dataset (`gld_price_data.csv`) contains:  
- **Date**: The date of the record  
- **SPX**: S&P 500 Index  
- **GLD**: Gold price  
- **USO**: Crude oil price  
- **SLV**: Silver price  
- **EUR/USD**: Exchange rate  

## Data Analysis & Preprocessing  
- **No missing values** found.  
- **Exploratory Data Analysis (EDA)** performed:  
  - Correlation heatmap to identify relationships.  
  - Distribution plot of gold prices.  
- **Feature selection**: Dropped the `Date` column and used numerical variables for prediction.  

## Model Training  
- **Features (X)**: `SPX`, `USO`, `SLV`, `EUR/USD`  
- **Target (Y)**: `GLD` (gold price)  
- **Train-Test Split**: 20% training, 80% testing  
- **Model Used**: **Random Forest Regressor** (n_estimators = 100)  

## Results  
- The **R² score** (coefficient of determination) of the model: **97.80%**  
- **Correlation Insights**:  
  - `SLV` (silver price) showed the highest positive correlation with gold prices (`0.86`).  
  - `USO` (crude oil price) had a negative correlation (`-0.18`).  
  - `SPX` and `EUR/USD` had weak correlations with gold prices.  

### Visualization  
- **Correlation Heatmap**: Displays relationships between features.  
- **Gold Price Distribution Plot**: Shows the distribution of `GLD` values.  
- **Actual vs. Predicted Plot**:  
  ![gold](https://github.com/user-attachments/assets/4724cabf-721f-4a08-980c-e067e6790a11)


## Dependencies  
- Python 3.x  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Scikit-learn  

## How to Run  
1. Install dependencies:  
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```  
2. Load the dataset (`gld_price_data.csv`).  
3. Run `gold_price_prediction.py` to train and test the model.  

## Author  
[mohit kumar]  
