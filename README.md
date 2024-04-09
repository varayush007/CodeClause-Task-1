# Bengaluru House Price Prediction

This project aims to build a linear regression model to predict house prices in Bengaluru based on various features such as the size of the house, total square feet, number of bathrooms, and location.

## Dataset

The dataset used in this project is the 'Bengaluru_House_Pricing.csv' file, which contains information about houses in Bengaluru, including their prices, sizes, total square feet, number of bathrooms, and locations.

## Dependencies

The following dependencies are required to run the code:

- pandas
- numpy
- scikit-learn
- matplotlib

## Code Explanation

1. **Data Loading and Preprocessing**
   - The dataset is loaded into a pandas DataFrame.
   - Missing values in the 'size' column are filled with the mode value, and missing values in the 'bath' column are filled with the median value.
   - Rows with missing values in the 'location' column are dropped.
   - The 'total_sqft' column is cleaned by removing non-numeric characters and handling ranges.
   - The 'size' column is converted to a numeric data type.

2. **Exploratory Data Analysis**
   - Box plots are generated for the 'size', 'total_sqft', 'bath', and 'price' columns to visualize the data distribution.

3. **Model Building**
   - The 'size' and 'total_sqft' columns are selected as features (X), and the 'price' column is the target variable (y).
   - The dataset is split into training and testing sets.
   - A linear regression model is created and evaluated using 5-fold cross-validation.
   - The cross-validation mean squared error (MSE), root mean squared error (RMSE), and R-squared score are printed.

4. **Model Fitting and Prediction**
   - The linear regression model is trained on the training data.
   - Predictions are made on the test data, and a new data point is used to demonstrate the prediction process.

## Usage

To run the code, simply execute the Python script. Make sure to have the 'Bengaluru_House_Pricing.csv' file in the same directory as the script, and ensure that all the required dependencies are installed.
