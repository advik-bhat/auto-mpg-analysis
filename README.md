# Auto MPG Analysis & Linear Regression

Exploratory data analysis, preprocessing, and linear regression on the Auto MPG dataset as part of the Coding Ninjas 10X Club AI/ML Recruitment Task.

## 📌 Overview

This project explores the Auto MPG dataset to understand the factors associated with vehicle fuel efficiency and builds Linear Regression models to predict MPG.

The project covers:

- Data exploration and statistical analysis
- Missing-value handling
- Duplicate detection and removal
- Data preprocessing
- Exploratory data visualization
- Correlation analysis
- Linear Regression
- Model evaluation
- Actual vs Predicted analysis
- Key findings and limitations

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## 📊 Dataset

The project uses the **Auto MPG** dataset from the UCI Machine Learning Repository.

The dataset contains information about vehicles including:

- MPG
- Cylinders
- Displacement
- Horsepower
- Weight
- Acceleration
- Model Year
- Origin
- Car Name

## 🔍 Exploratory Data Analysis

The analysis investigates:

- Distribution of MPG
- Relationship between MPG and displacement
- Relationship between MPG and horsepower
- Relationship between MPG and vehicle weight
- Relationship between MPG and acceleration
- MPG across different cylinder groups
- MPG trends across model years
- Correlations between numerical variables
- Unusual observations and potential outliers

## 🤖 Machine Learning

Two Linear Regression models were developed:

### 1. Weight-only Model

A baseline model using vehicle weight as the single predictor of MPG.

### 2. Multiple-feature Model

A model using multiple vehicle characteristics to predict MPG.

The `car_name` column was removed and `origin` was one-hot encoded before modelling.

The dataset was split into:

- 80% training data
- 20% testing data
- `random_state = 42`

## 📈 Evaluation Metrics

The models were evaluated using:

- MAE — Mean Absolute Error
- MSE — Mean Squared Error
- RMSE — Root Mean Squared Error
- R² — Coefficient of Determination

An Actual vs Predicted MPG plot was also used to visually evaluate model performance.

## 💡 Key Insights

Some major observations from the analysis include:

- Vehicle weight has a strong relationship with fuel efficiency.
- Larger engine displacement is generally associated with lower MPG.
- Higher horsepower tends to be associated with lower MPG.
- Cylinder count is related to differences in fuel efficiency.
- Average MPG shows an overall positive relationship with model year.
- Multiple vehicle characteristics provide more information for MPG prediction than weight alone.

## 📁 Repository Structure

```text
auto-mpg-analysis/
│
├── Auto_MPG_Analysis_Linear_Regression.ipynb
├── auto_mpg_cleaned.csv
└── README.md
