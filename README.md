# House Price Prediction

## Overview

This project was developed as part of the **Xylofy AI Week 1 Internship Project**. The objective is to predict house prices using machine learning techniques and identify the factors that have the greatest influence on property value.

The project includes data exploration, preprocessing, visualization, model building, performance evaluation, and feature importance analysis.

---

## Dataset

**Source:** Kaggle Housing Prices Dataset

* Total Records: 545
* Target Variable: `price`
* Features:

  * area
  * bedrooms
  * bathrooms
  * stories
  * mainroad
  * guestroom
  * basement
  * hotwaterheating
  * airconditioning
  * parking
  * prefarea
  * furnishingstatus

Dataset Link:

https://www.kaggle.com/datasets/yasserh/housing-prices-dataset

---

## Project Workflow

### 1. Data Loading and Exploration

* Loaded dataset using Pandas
* Displayed sample records
* Checked dataset dimensions
* Identified features and target variable
* Checked missing values

### 2. Data Preprocessing

* Verified missing values
* Removed duplicate records
* Applied One-Hot Encoding to categorical features
* Prepared data for machine learning models

### 3. Model Development

Two regression models were trained:

#### Linear Regression

A simple regression model used as the baseline approach.

#### Random Forest Regressor

An ensemble learning method based on multiple decision trees.

---

## Model Performance

| Model             | MAE     | RMSE    | R² Score |
| ----------------- | ------- | ------- | -------- |
| Linear Regression | 970043  | 1324507 | 0.6529   |
| Random Forest     | 1013969 | 1398116 | 0.6133   |

### Best Model

**Linear Regression** achieved the best performance with an R² score of approximately **0.65**.

---

## Visualizations

The following visualizations were created:

1. House Price Distribution
2. Correlation Heatmap
3. House Price by Furnishing Status
4. Actual vs Predicted Prices (Linear Regression)
5. Actual vs Predicted Prices (Random Forest)
6. Random Forest Feature Importance

---

## Key Findings

* Area is the most influential factor affecting house price.
* Bathrooms significantly impact property value.
* Air conditioning, parking, and stories also contribute to price.
* Furnished houses generally have higher prices.
* Bedrooms had less influence than expected.
* Linear Regression slightly outperformed Random Forest on this dataset.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## Project Structure

```text
HousePricePrediction_MohammadZuheer/
│
├── analysis.ipynb
├── Housing.csv
├── summary.pdf
├── README.md
│
└── charts/
    ├── 01_House_Price_Distribution.png
    ├── 02_Correlation_Heatmap.png
    ├── 03_House_Price_by_Furnishing_Status.png
    ├── 04_Actual_vs_Predicted_Linear_Regression.png
    ├── 05_Actual_vs_Predicted_Random_Forest.png
    └── 06_Random_Forest_Feature_Importance.png
```

---

## Conclusion

This project demonstrates how machine learning can be used to estimate house prices based on property characteristics. The analysis highlights the importance of area, bathrooms, and amenities in determining house value and provides useful insights for real estate pricing decisions.

---

## Author

**Mohammad Zuheer**

B.Tech, Materials Science and Engineering
Indian Institute of Technology (IIT) Mandi
