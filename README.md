# Insurance Cost Prediction 🏥💰

This project implements a machine learning model to predict individual medical insurance costs using **Linear Regression** optimized with a **Genetic Algorithm (GA)**.

## 📌 Project Overview
The goal is to predict healthcare expenses based on personal attributes such as age, BMI, number of children, and smoking status. This helps insurance companies determine fair premiums.

## 👥 Authors
- **Jian Hazel Sitorus**
- **Mikhael Restu Mahardhika**

## 📂 Dataset
The project uses the **Medical Cost Personal Datasets** (`insurance.csv`) from Kaggle.
- **Features Used**:
  - `age`: Age of primary beneficiary.
  - `bmi`: Body mass index.
  - `children`: Number of children covered by health insurance.
  - `smoker`: Smoking status (Encoded: yes=1, no=0).
- **Target**: `charges` (Medical insurance costs).

> **Note**: `sex` and `region` columns are present in the original dataset but were excluded from this model's training process as they showed lower correlation.

## 🛠️ Methodology
1. **Data Preprocessing**:
   - Encoding categorical variables (e.g., `smoker` -> 0/1).
   - Normalization (Min-Max Scaling) to bring features to a 0-1 range.
   - Manual Train-Test Split (80% Train, 20% Test).

2. **Model**:
   - **Linear Regression**: Implemented from scratch.
   - **Optimization**: **Genetic Algorithm (GA)** is used to find the optimal weights ($w$) and bias ($b$) for the regression model, minimizing the error (MSE).

## 🚀 How to Run
1. Ensure you have Python installed with the following libraries:
   - `pandas`
   - `numpy`
   - `matplotlib`
   - `seaborn`
   - `scikit-learn` (for metrics comparison)
2. Open `Insurance_Cost_Prediction.ipynb` in Jupyter Notebook or Google Colab.
3. Run the cells sequentially to see the data analysis, training process, and prediction results.

## 📊 Results
The notebook demonstrates the evolution of the model's fitness over generations and visualizes the predicted vs. actual insurance charges.
