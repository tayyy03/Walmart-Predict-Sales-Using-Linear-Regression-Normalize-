# Walmart-Predict-Sales-Using-Linear-Regression-Normalize-

This project is about predicting sales for the next 30 days based on features such as 'Temperature', 'Fuel_Price', 'CPI', 'Unemployment', and 'Store'. The model used for this prediction is Linear Regression.

## Dependencies

- pandas
- sklearn
- matplotlib
- tabulate

## How to Run

1. Ensure that you have all the dependencies installed.
2. Run the `sales_store_predict.ipynb` notebook.

## Code Overview

The code first defines the features and target from the dataframe `df`. It then splits the data into training and testing sets.

The features are then scaled using `StandardScaler` from `sklearn.preprocessing`.

A Linear Regression model is trained on the scaled training data and predictions are made on the scaled testing data.

The code then prepares for future predictions by converting the 'Date' column to datetime and creating a new 'Date_ordinal' column.

For the next 30 days, the code selects the features for each day, scales them, and makes a prediction using the trained model. These predictions are stored in `pred_list`.

The predictions are then tabulated and plotted.

## Output

The output is a table of sales predictions for the next 30 days and a plot of these predictions.

## Dataset
https://www.kaggle.com/datasets/yasserh/walmart-dataset
