# CarPricePrediction

# 🚗 Car Price Prediction

This project focuses on predicting the prices of used cars using **Linear Regression** and **Lasso Regression** models. It aims to provide an end-to-end machine learning pipeline—from data preprocessing and exploratory analysis to model training, evaluation, and interpretation.

---

## 📊 Problem Statement

With the rise of the second-hand car market, pricing used cars accurately is a valuable service for buyers and sellers. The objective is to build regression models that predict car prices based on various features such as brand, year of manufacture, mileage, fuel type, transmission, etc.

---

## 🛠️ Tech Stack

- **Python**
- **Pandas**, **NumPy** – Data manipulation
- **Matplotlib**, **Seaborn** – Data visualization
- **Scikit-learn** – Machine Learning (Linear & Lasso Regression)
- **Jupyter Notebook**

---

## 🔍 Dataset Overview

The dataset contains features like:
- `Car_Name`
- `Year`
- `Selling_Price`
- `Present_Price`
- `Kms_Driven`
- `Fuel_Type`
- `Seller_Type`
- `Transmission`
- `Owner`

> 📌 Target Variable: `Selling_Price`

---

## 🧼 Data Preprocessing

- Handling missing values
- Encoding categorical variables (`Fuel_Type`, `Seller_Type`, `Transmission`)
- Feature scaling
- Outlier detection
- Feature selection using correlation matrix

---

## 📈 Model Building

### 1. Linear Regression
- Baseline model to understand data relationships
- Evaluated using **R² score**, **MAE**, and **MSE**

### 2. Lasso Regression
- Regularized linear model to reduce overfitting
- Used to eliminate less important features (L1 penalty)

---

## 🧪 Model Evaluation

- **Train-Test Split**
- **Cross-validation (K-Fold)**
- **Performance Metrics:**
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - R² Score

| Model            | R² Score | MAE     | MSE     |
|------------------|----------|---------|---------|
| Linear Regression| 0.91     | 1.05    | 2.02    |
| Lasso Regression | 0.90     | 1.10    | 2.18    |

> ⚖️ Lasso helped reduce overfitting and improved generalization.

---

## 📌 Key Insights

- **Present Price** and **Year** are strong predictors.
- Cars with manual transmission tend to have lower prices.
- Lasso Regression effectively reduced model complexity without major performance loss.

---

## 📂 Project Structure

car-price-prediction/ │ ├── data/ # Dataset CSV ├── notebooks/ # Jupyter notebooks │ ├── EDA.ipynb # Exploratory Data Analysis │ ├── Linear_Regression.ipynb │ └── Lasso_Regression.ipynb ├── models/ # Trained model files (pickle) ├── images/ # Plots and visualizations └── README.md

---

## 🚀 Future Work

- Hyperparameter tuning using GridSearchCV
- Add more advanced models (Ridge, ElasticNet, XGBoost)
- Deploy as a web app using Flask/Streamlit

---

## 👨‍💻 Author

**Rahul Pandey**  
📧 rahulpandey02124@gmail.com 
🔗 https://github.com/rahulpandey535

---

## 📜 License

This project is licensed under the MIT License.
