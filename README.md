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

The EDA shows distribution of data and relation between different features' Below are few highlights from the tables:

![alt text](https://github.com/davideragone/Adult_Census_-Income_-Project/blob/main/Pictures/bar_occupation.png "Different Occupations")
![alt text](https://github.com/davideragone/Adult_Census_-Income_-Project/blob/main/Pictures/corr_matrix.png "Correlation Matrix")
![alt text](https://github.com/davideragone/Adult_Census_-Income_-Project/blob/main/Pictures/pie_plot_education.png "Education pie chart")


## Data Cleaning

Create a `preprocess_data(df)` function that performs transformations on the DataFrame given as parameter and returns its converted version. Below the changes function makes:

* Fill missing numerical values with feature median
* Convert Object data into numerical
* For each feature with missing data, creates a binary column with Boolean values (True where missing, False where not missing)

## Model Building 

* Split Data into `train` and `test` data
* Create `fit_and_score` function to instantiate and get accuracy from different estimators at the same time
* 5 different models used:
KNeighbors Classifier 
Logistic Regression
Random Forest Classifier
XGBoost Classifier
CatBoost Classifier
* Hyperparameter tuning using RandomizedSearchCV and GRidSearchCV for the two best performant classifier

## Model Performance

* Metrics evaluation using Cross Validation (Precision, Recall and F1 scores), ROC curve and AUC, Confusion Matrix and Classification Report
* Feature Importance
