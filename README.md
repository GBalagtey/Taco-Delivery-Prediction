# 🌮 Taco Delivery Duration Prediction

Predicting taco delivery times using machine learning techniques on a real-world styled dataset. This project demonstrates end-to-end ML workflow including data preprocessing, feature engineering, model building, and evaluation.

## 📦 Dataset

This project uses the **Taco Sales Dataset (2024–2025)** by Atharva Soundankar from [Kaggle](https://www.kaggle.com/datasets/atharva32/taco-sales-dataset-20242025). It includes detailed records of taco orders placed in the U.S., featuring:

- Order ID
- Restaurant Name
- Location
- Order Time
- Delivery Time
- Taco Size & Type
- Toppings Count
- Distance (km)
- Price ($)
- Tip ($)
- Weekend Order indicator

The target variable is:

- `Delivery Duration (min)` – total delivery time in minutes.

## 🛠 Features Used

After cleaning and transformation, the following features were selected for model training:

- `Taco Size`
- `Taco Type`
- `Toppings Count`
- `Distance (km)`
- `Price ($)`
- `Tip ($)`
- `Weekend Order`
- `hour` (from Order Time)
- `dayofweek` (mapped numerically)
- `is_weekend`

Categorical variables were one-hot encoded and time-based features were extracted for better predictive performance.

## 🧠 Models Developed

Three main regression models were evaluated:

- **Linear Regression**
- **Random Forest Regressor**
- **Gradient Boosting Regressor**

### Feature Importance Techniques Applied:
- Linear Regression Coefficients
- Random Forest Feature Importances
- Gradient Boosting Feature Importances

## 📈 Evaluation Metrics

The models were evaluated using:

- **MAE** (Mean Absolute Error)
- **MSE** (Mean Squared Error)
- **RMSE** (Root Mean Squared Error)

8-fold cross-validation was used for robust performance comparison.

## 📊 Results

Model performance across MAE, MSE, and RMSE was recorded. Random Forest and Gradient Boosting models generally outperformed Linear Regression due to their ability to capture non-linear relationships.

*(Insert performance table or graph here, if available in the notebook)*

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/taco-delivery-prediction.git
   cd taco-delivery-prediction
