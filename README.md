# foodnutrientdataset_multilinearregression
# 🍎 Food Nutrient Dataset – Multiple Linear Regression

## 📌 Project Overview

This project demonstrates the use of **Multiple Linear Regression** to analyze and predict nutritional values in food items. The model uses multiple independent variables such as calories, protein, and fat to predict a dependent variable (e.g., carbohydrates).

---

## 📂 Dataset Description

The dataset contains nutritional information about different food items.

### 🔑 Features (Independent Variables)

* **Calories** – Total energy content in food
* **Protein** – Amount of protein (grams)
* **Fat** – Amount of fat (grams)

### 🎯 Target Variable (Dependent Variable)

* **Carbohydrates** – Amount of carbohydrates (grams)

---

## 🎯 Objective

To build a **Multiple Linear Regression model** that predicts the carbohydrate content based on:

* Calories
* Protein
* Fat

---

## 🧮 Model Used

We use **Multiple Linear Regression**, which is an extension of simple linear regression with more than one input variable.

### 📘 Equation:

Carbohydrates = b₀ + b₁(Calories) + b₂(Protein) + b₃(Fat)

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🚀 Steps Involved

1. Import libraries
2. Load dataset using Pandas
3. Explore data (head, info, describe)
4. Split dataset into:

   * Independent variables (X)
   * Dependent variable (y)
5. Train-test split
6. Train model using LinearRegression
7. Predict values
8. Evaluate model performance

---

## 📊 Data Visualization

* Scatter plots
* Pair plots using Seaborn
* Heatmap for correlation

---

## 📈 Model Evaluation Metrics

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* R² Score

---

## ▶️ Example Code Snippet

```python
from sklearn.linear_model import LinearRegression
import pandas as pd

# Load dataset
data = pd.read_csv('food_nutrient.csv')

# Independent variables
X = data[['Calories', 'Protein', 'Fat']]

# Dependent variable
y = data['Carbohydrates']

# Model
model = LinearRegression()
model.fit(X, y)

# Prediction
predictions = model.predict(X)
```

---

## 📌 Conclusion

This project shows how multiple factors influence a single outcome. Multiple Linear Regression helps in understanding relationships between nutritional components and predicting unknown values.

---

## 📎 Future Improvements

* Add more features (fiber, sugar, vitamins)
* Use larger dataset
* Apply advanced models (Random Forest, XGBoost)

---

## 👨‍💻 Author

Your Name

---
