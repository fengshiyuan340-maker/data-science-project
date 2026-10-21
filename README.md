# Laptop Price Prediction Project

## Problem / Research Question
How can we accurately predict the price of a laptop based on its hardware specifications (like CPU frequency, RAM, storage, etc.)? This project explores single linear regression, multiple linear regression, and polynomial regression techniques to find the best-performing model.

## Dataset Source and Permissions
The dataset (`laptops.csv`) is a publicly available dataset used for educational purposes in the CISC7204 course. It contains 238 rows and 12 features. No sensitive or personal data is included.

## Methods and Tools Used
*   **Language:** Python
*   **Libraries:** Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib
*   **Methods:** 
    *   Simple Linear Regression (CPU frequency vs. Price)
    *   Multiple Linear Regression (7 features)
    *   Polynomial Regression (Degrees 1, 3, 5)
    *   Machine Learning Pipeline with StandardScaler and PolynomialFeatures

## Key Findings and One Limitation
*   **Key Findings:** The multiple linear regression and polynomial pipeline significantly improved the training R² score (from 0.134 to 0.633) compared to single linear regression. CPU frequency alone is not enough to explain price variance.
*   **Limitation:** All evaluations are in-sample (training data). The polynomial models may overfit the training data, meaning their real-world performance on unseen laptops might be worse.

## Instructions for Running the Analysis
1. Clone this repository.
2. Install the required packages: `pip install -r requirements.txt`
3. Ensure `laptops.csv` is in the same directory.
4. Open and run the Jupyter Notebook (`.ipynb` file) to see the analysis and visualizations.
