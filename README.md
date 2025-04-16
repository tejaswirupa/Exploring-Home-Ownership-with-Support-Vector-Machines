# Predicting Home Ownership Using Support Vector Machines (SVM)

## Overview
This project investigates the factors influencing home ownership using **Support Vector Machines (SVM)** with linear, radial, and polynomial kernels. Based on data from the **Integrated Public Use Microdata Series (IPUMS USA)**, this model aims to uncover how demographic and housing factors affect ownership status and provide insights for housing policy improvements.

---

## Objectives
- Predict home ownership status using SVM classifiers
- Compare kernel performances: Linear, Radial Basis Function (RBF), and Polynomial
- Identify top features influencing ownership (e.g., bedrooms, age, number of families)
- Explore social and economic implications of model findings

---

## Methods
- **Data Cleaning**: Handled duplicates, irrelevant columns, and categorized key attributes
- **Modeling**:
  - Linear Kernel: Grid search for optimal `C`
  - Radial Kernel: Tuned `C` and `gamma`
  - Polynomial Kernel: Tuned `C` and polynomial `degree`
- **Evaluation**:
  - Accuracy Scores: Linear (82.80%), Radial (83.48%), Polynomial (83.07%)
  - Feature importance via coefficient magnitude and kernel sensitivity
  - Decision boundary plots for each kernel type

---

## Key Results
| Kernel      | Accuracy | Top Features                    |
|-------------|----------|---------------------------------|
| Linear      | 82.80%   | Bedrooms, Number of Families    |
| Radial      | 83.48%   | Age, Bedrooms                   |
| Polynomial  | 83.07%   | Bedrooms, Age                   |

- The **number of bedrooms** consistently appeared as the most impactful feature across all kernels.
- **Age** and **household size** also play key roles in ownership likelihood.

---

## Societal Impact
- Larger households and younger individuals may face **more barriers** to home ownership.
- Findings suggest policy support could focus on **first-time homebuyers** and **family-sized housing units**.

---

## Tools & Technologies
- Python (Scikit-learn, Pandas, Matplotlib)
- SVM Kernels: Linear, RBF, Polynomial
- GridSearchCV for parameter tuning
- IPUMS USA Housing Dataset

---
