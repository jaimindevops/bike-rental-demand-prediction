# Bike Sharing Demand Modeling

The project investigates the Bike Sharing Dataset and creates predictive models for daily and hourly rental counts. The entire process of data loading, cleaning, exploring, feature engineering, and model training is conducted through the notebook.

## 1. Project Scope

-   Daily and hourly datasets are loaded and inspected
-   Missing values, duplicates, and parsing issues are checked
-   Exploratory analysis is run on weather, seasonality, and time features
-   Features are engineered for model readiness
-   Multiple regression models are trained
-   Model performances are compared using error metrics

## 2. Requirements

Install dependencies:

``` bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 3. Dataset

This notebook uses the UCI Bike Sharing Dataset:

-   `day.csv` --- daily aggregated data
-   `hour.csv` --- hourly-level data

Place these files in the same directory as the notebook.

## 4. Notebook Structure

### A. Initialization

Import the libraries and set the configurations for plotting/display.

### B. Data Loading

Use `pandas.read_csv()` to import daily and hourly datasets and examine their basic characteristics/samples.

### C. Data Inspection

-   Check for missing values
-   Data comparators for duplicates
-   Date parsing and validation
-   Metadata and statistical summaries

### D. Exploratory Analysis

Data visualizations and patterns built are:
- Weather effects
- Seasonality
- Casual vs. Registered Users
- Hourly and Daily Demand Trends

### E. Feature Engineering

Typical steps:
- Convert and extract date/time components.
- One-hot encoding of the categorical variables.
- Generate additional relevant features.

### F. Model Training

The notebook trains the following models:
- Random Forest Regressor
- Long Short-Term Memory (LSTM)

The models are evaluated using below methods:
- RMSE
- MAE
- MSE

### G. Results

Summarizing the model accuracy, feature importance, and final recommendations.

## 5. How to Run

1.  Put the files `day.csv`, `hour.csv`, and the notebook together in one folder.
2.  Launch the notebook either in Jupyter or VSCode.
3.  Run all the cells sequentially.
4.  Check the results of the final model evaluation.

## 6. Output

You will get:
- Cleaned datasets
- EDA visuals
- A number of trained models after modelling
- Comparisons of error metrics
- Insights into demand drivers
