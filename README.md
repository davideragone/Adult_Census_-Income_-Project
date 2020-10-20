# Adult_Census_-Income_-Project
Repo for the Adult Census Income Project 
# Project Overview

* Exploratory Data Analysis, outliers identification and data cleaning.

* Modelling using KNeighbors, Logistic Regression, Random Fores, CatBoost amd XGBoost classifiers.

* Hyperparameters tuning usings RandomizedSearchCV amd  GridSearchCV.

* Metrics evaluation and Feature Importance.

## Code and Resourses used

**Python Version:** 3.8.2

**Packages:** Pandas, Numpy, Matplotlib, Seaborn, SKlearn, XGBoost, CatBoost

## EDA: Exploratory Data Analysis

The EDA shows distribution of data and relation between different features' Below some highlights pulled out from it:

![alt text] (https://github.com/davideragone/Adult_Census_-Income_-Project/blob/main/Pictures/bar_occupation.png "Different Occupations")






## Data Cleaning

Create a `preprocess_data(df)` function that performs transformations on the DataFrame given as parameter and returns its converted version. Below the changes function makes:

* Fill missing numerical values with feature median
* Convert Object data into numerical
* For each feature with missing data, creates a binary column with Boolean values (True where missing, False where not missing)
