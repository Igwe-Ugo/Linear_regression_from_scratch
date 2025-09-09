# 📘 Linear Regression from Scratch in Python

This project is a **from-scratch implementation of Linear Regression** using only **NumPy**, without relying on high-level machine learning libraries such as Scikit-Learn or TensorFlow. It demonstrates both **single-variable** and **multiple-variable** regression, and compares results against Scikit-Learn’s `LinearRegression` for validation.

---

## 🚀 Features

* Implemented **gradient descent** for parameter optimization.
* Supports:

  * **Single-feature regression** (e.g., `MedInc → MedHouseVal`)
  * **Multiple-feature regression** (all 8 features of the California Housing dataset)
* Calculates evaluation metrics:

  * Mean Squared Error (MSE)
  * Root Mean Squared Error (RMSE)
  * Mean Absolute Error (MAE)
  * R² Score
* Visualizations:

  * Regression line for single-feature case.
  * Predicted vs actual scatter plot for multiple features.
  * Cost function convergence plot.
* Validated against **Scikit-Learn** results.

---

## 📊 Results Summary

### ✅ Single Feature (Median Income → Median House Value)

* **From Scratch:** R² ≈ 0.4589
* **Scikit-Learn:** R² ≈ 0.4589
* Parameters nearly identical (`w ≈ 0.6904`, `b ≈ -0.0007`)

### ✅ Multiple Features (All 8 Features → Median House Value)

* **From Scratch:** R² ≈ 0.5775
* **Scikit-Learn:** R² ≈ 0.5758
* Both models produced almost identical error metrics.

📌 Takeaway: Gradient descent from scratch matches Scikit-Learn’s Ordinary Least Squares implementation, and adding more features significantly improves model performance.

---

## 📂 Project Structure

```
linear_regression_from_scratch/
│── data/                  # Dataset (California Housing from sklearn.datasets)
│── linear_regression_from_scratch.py   # Main implementation
│── plots/                 # Visualizations (regression lines, cost curves, residuals)
│── README.md              # Project documentation
```

---

## ⚙️ Installation & Usage

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/linear_regression_from_scratch.git
   cd linear_regression_from_scratch
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

   *(Required: `numpy`, `matplotlib`, `scikit-learn`)*

3. Run the script:

   ```bash
   python linear_regression_from_scratch.py
   ```

---

## 📈 Example Plots

### Single Feature Regression

Scatter plot with regression line (`MedInc → MedHouseVal`).

### Multiple Feature Regression

Predicted vs actual scatter plot and cost curve showing gradient descent convergence.

---

## 🔬 Learning Outcomes

* Hands-on understanding of **gradient descent** for optimization.
* Difference between **iterative gradient descent** and **closed-form OLS solution**.
* Importance of using multiple features for better predictive performance.
* How to evaluate regression models beyond accuracy (MSE, RMSE, MAE, R²).

---

## 📚 References

* [Scikit-Learn Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html)
* Andrew Ng’s Machine Learning course
* California Housing Dataset (`sklearn.datasets.fetch_california_housing`)

---

## ✍️ Author

Developed by **Igwe Ugochukwu Edwin (https://github.com/Igwe-Ugo)** — as part of my journey to deeply understand **Machine Learning fundamentals by building models from scratch**.

