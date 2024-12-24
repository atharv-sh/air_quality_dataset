# Air Quality Index Prediction

This Jupyter Notebook explores air quality index (AQI) prediction using various machine learning models.

## Data

The notebook uses a CSV file named 'data_date.csv' (not included in this repository). This file is expected to contain features related to air quality, including:

* Date
* AQI Value
* Status (e.g., Good, Moderate, Unhealthy)
* Country
* Other relevant features

## Data Preprocessing

The notebook performs the following preprocessing steps:

* Converts the 'Date' column to datetime objects.
* Encodes the categorical 'Status' column using one-hot encoding.
* Scales the numerical features using MinMaxScaler.

## Exploratory Data Analysis (EDA)

The notebook includes various visualization techniques to explore the data, such as:

* Line plots of AQI over time
* Histograms and box plots of AQI distributions
* Correlation matrix heatmap
* Pair plots of features
* Scatter plots, bar plots and violin plots

## Model Training and Evaluation

The notebook trains several regression models, including:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor
* Support Vector Regression

The models are evaluated using Mean Squared Error (MSE) and R-squared metrics.  The best-performing model (based on R-squared) is saved for later use.

## Model Deployment

The trained model is saved using `joblib` as 'best_model.pkl'.  Sample code is provided to load the saved model and make predictions on new data.

## Usage

1.  Ensure you have the necessary libraries installed (see requirements.txt)
2.  Place your 'data_date.csv' file in the same directory as the notebook.
3.  Run the notebook cells sequentially.

## Dependencies

The following libraries are used in this notebook:

* numpy
* pandas
* matplotlib
* seaborn
* scikit-learn
* joblib
