# Car Price Prediction Using Linear Regression

## Project Overview

This project focuses on predicting car prices using a Linear Regression machine learning model.

The project includes Exploratory Data Analysis (EDA), data preprocessing, feature scaling, categorical encoding, model training, model evaluation, residual analysis, and model improvement.

## Dataset

The dataset contains information about different cars and their prices.

The features used in the final model include:

- Engine size
- Horsepower
- Curb weight
- Drive wheels
- Manufacturer

The target variable is **price**.

## Exploratory Data Analysis

Exploratory Data Analysis was performed to understand the relationships, distributions, and patterns present in the dataset.

Key observations:

- Engine size, horsepower, and curb weight show strong positive relationships with car price.
- Car prices vary across different drive-wheel categories.
- Car prices vary across different manufacturers.
- The numerical features show some correlation with each other.

## Data Preprocessing

The following preprocessing steps were performed:

- Selected relevant features for modelling.
- Separated features and target variable.
- Split the data into training and testing sets.
- Classified features into numerical and categorical variables.
- Scaled numerical features using `StandardScaler`.
- Encoded categorical features using `OneHotEncoder`.

## Model Development

### Baseline Model

A baseline Linear Regression model was trained using:

- Engine size
- Horsepower
- Curb weight
- Drive wheels

The baseline model achieved an **R² score of 0.8355** on the test data.

### Improved Model

The model was improved by adding **manufacturer** as an additional feature.

The improved model achieved an **R² score of 0.8747** on the test data.

## Model Evaluation

The models were evaluated using:

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

### Model Comparison

| Metric | Baseline Model | Improved Model |
|---|---:|---:|
| R² | 0.8355 | 0.8747 |
| MAE | ~2,513 | ~2,138 |
| MSE | ~12,984,889 | ~9,889,464 |
| RMSE | ~3,603 | ~3,144 |

The improved model performed better across all evaluation metrics.

## Residual Analysis

Residual analysis was performed to understand the prediction errors of the model.

The residuals were generally distributed around zero, although some variation, clustering, and a few large residuals were observed.

## Final Model

The improved Linear Regression model was selected as the final model because it provided better performance than the baseline model.

The final model explains approximately **87.47% of the variation in car prices** on the test data.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

## Project Structure

```text
Car Price Prediction Linear Regression Model/
│
├── Car Price Prediction Linear Regression Model.ipynb
├── scrap price.csv
├── README.md
├── .gitignore
└── LICENSE
