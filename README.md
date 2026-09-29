# Auto MPG Analysis & Linear Regression

Exploratory data analysis, preprocessing, and linear regression on the Auto MPG dataset as part of the **Coding Ninjas 10X Club AI/ML Recruitment Task 2026**.

## 🔗 Project Links

- 📓 [Google Colab Notebook](https://colab.research.google.com/drive/1UiXBnA3A7A9YTX5vU14Jovbdkp8ZeB1B?usp=sharing)
- 📊 [Cleaned Dataset](./auto_mpg_cleaned.csv)

> The Google Colab notebook contains the complete data exploration, preprocessing, visualizations, regression models, evaluation metrics, and analysis.

---

## 📌 Overview

This project analyzes the **Auto MPG** dataset to understand the factors associated with vehicle fuel efficiency and builds Linear Regression models to predict miles per gallon (MPG).

The project covers:

- Data exploration and statistical analysis
- Data cleaning and preprocessing
- Missing-value handling
- Duplicate detection and removal
- Exploratory Data Analysis (EDA)
- Data visualization
- Correlation analysis
- Linear Regression
- Model evaluation
- Actual vs Predicted analysis
- Key findings and limitations

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Scikit-learn**
- **Google Colab**

---

## 📊 Dataset

The project uses the **Auto MPG** dataset from the **UCI Machine Learning Repository**.

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

The `car_name` column is removed before model training, while `origin` is treated as a categorical feature and one-hot encoded.

### Dataset Reference

Quinlan, R. (1993). *Auto MPG*. UCI Machine Learning Repository.

---

## 🔍 Exploratory Data Analysis

The analysis investigates:

- Distribution of MPG
- MPG vs displacement
- MPG vs horsepower
- MPG vs vehicle weight
- MPG vs acceleration
- MPG across different cylinder groups
- MPG trends across model years
- Correlations between numerical variables
- Unusual observations and potential outliers

### Key Questions Explored

- How is MPG distributed across the dataset?
- Which vehicle characteristics are most strongly associated with MPG?
- How does fuel efficiency vary across cylinder groups?
- Did average fuel efficiency change across model years?
- How well can MPG be predicted using vehicle characteristics?

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. Converted relevant columns to appropriate numeric data types.
2. Identified missing values.
3. Handled missing `horsepower` values using median imputation.
4. Checked for duplicate records and removed exact duplicates.
5. Checked for physically impossible numeric values.
6. Investigated unusual observations without automatically removing legitimate extreme values.
7. Removed `car_name` before machine learning.
8. One-hot encoded the categorical `origin` feature.

The cleaned dataset is included in this repository as:

`auto_mpg_cleaned.csv`

---

## 🤖 Machine Learning

Two Linear Regression models were developed.

### 1. Weight-Only Model

A baseline Linear Regression model using **vehicle weight** as the only predictor of MPG.

This provides a simple baseline for comparison.

### 2. Multiple-Feature Model

A Linear Regression model using multiple vehicle characteristics to predict MPG.

The model uses:

- Cylinders
- Displacement
- Horsepower
- Weight
- Acceleration
- Model Year
- One-hot encoded Origin

The dataset was divided into:

- **80% training data**
- **20% testing data**

with:

```text
random_state = 42




## 📚 References

- Quinlan, R. (1993). Auto MPG. UCI Machine Learning Repository.
- UCI Machine Learning Repository — Auto MPG Dataset
  https://doi.org/10.24432/C5859H


## 👤 Author

### Advik Bhat
