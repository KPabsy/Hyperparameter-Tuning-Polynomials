# Polynomial Regression & Hyperparameter Tuning

This repository explores the fundamentals of **Polynomial Regression**, specifically focusing on how model complexity affects performance. Using a synthetic cubic dataset, the project demonstrates the process of **Hyperparameter Tuning** by comparing different polynomial degrees to find the optimal balance between underfitting and overfitting.

## 🚀 Project Overview

The primary goal of this analysis is to determine the best polynomial degree for a non-linear dataset. We evaluate the model's performance across four different degrees of complexity:

* **Degree 1:** Linear Regression (Simple line)
* **Degree 2:** Quadratic Regression (Simple curve)
* **Degree 3:** Cubic Regression (The "True" model)
* **Degree 10:** High-degree Polynomial (Complex curve)

## 📊 Key Concepts Demonstrated

### 1. The Bias-Variance Tradeoff

* **Underfitting (Degree 1):** The model is too simple to capture the underlying pattern of the data, resulting in low training and validation scores.
* **Optimal Fit (Degree 3):** The model matches the complexity of the data generation function, resulting in high accuracy on both training and validation sets.
* **Overfitting (Degree 10):** The model becomes too sensitive to random noise in the training data, potentially leading to poor generalization on new data.

### 2. Data Splitting Strategy

To ensure a robust evaluation, the data is split into three parts:

* **Training Set (60%):** To fit the models.
* **Validation Set (20%):** To compare different hyperparameters (degrees) and select the best one.
* **Test Set (20%):** Reserved for final unbiased evaluation.

## 🛠️ Requirements

To run this notebook, you will need:

* **Python 3.x**
* **Jupyter Notebook** or **Google Colab**
* Libraries: `numpy`, `pandas`, `matplotlib`, `scikit-learn`

## 📈 Results Summary

| Model Degree | Training Score () | Validation Score () | Interpretation |
| --- | --- | --- | --- |
| **1** | ~0.61 | ~0.58 | Underfit |
| **2** | ~0.89 | ~0.86 | Better fit |
| **3** | ~0.99 | ~0.99 | **Optimal Fit** |
| **10** | ~0.99 | ~0.99 | Potential Overfit |

## 📜 Usage

1. Clone the repository.
2. Open `Polynomial_Regression_Tuning.ipynb` (or your chosen filename).
3. Run the cells sequentially to generate the data, train the models, and view the comparison plots.

---
