# 🌿 Energy Efficiency Prediction

> Predicting Heating and Cooling Loads of Buildings using Machine Learning

[📂 Dataset Source (UCI ML Repo)](https://archive.ics.uci.edu/dataset/242/energy+efficiency)

---

## 📌 Project Overview

This study aims to assess the **heating load** and **cooling load** requirements of buildings (i.e., energy efficiency) based on various **building parameters**. Using simulations from Ecotect for 12 building shapes under various conditions, the dataset includes:

- **768 samples**
- **8 features** (X1 to X8)
- **2 target variables**:
  - `Y1`: Heating Load  
  - `Y2`: Cooling Load

---

## 🧪 Dataset Summary

> The buildings vary in glazing area, orientation, surface area, etc., and the dataset can be used for both regression and multi-class classification (if targets are rounded).

| Name | Role    | Type       | Description                   |
|------|---------|------------|-------------------------------|
| X1   | Feature | Continuous | Relative Compactness          |
| X2   | Feature | Continuous | Surface Area                  |
| X3   | Feature | Continuous | Wall Area                     |
| X4   | Feature | Continuous | Roof Area                     |
| X5   | Feature | Continuous | Overall Height                |
| X6   | Feature | Integer    | Orientation                   |
| X7   | Feature | Continuous | Glazing Area                  |
| X8   | Feature | Integer    | Glazing Area Distribution     |
| Y1   | Target  | Continuous | Heating Load                  |
| Y2   | Target  | Continuous | Cooling Load                  |

---

## 📊 Visualizations

### 🔍 Input Feature Distribution
<img width="936" height="790" alt="Feature Distribution" src="https://github.com/user-attachments/assets/9fb4b4fe-741c-49d3-b824-b2bf0e25fc22" />

### 📈 Model Predictions vs True Values
<img width="2485" height="2490" alt="Model Performance" src="https://github.com/user-attachments/assets/77a7fe32-7792-4ebe-8780-8c0e02b48e69" />

---

## 🤖 Model Performance Comparison

| Model                    | MSE   | R² (Heating Load) | R² (Cooling Load) |
|--------------------------|-------|-------------------|-------------------|
| Linear Regression        | 9.52  | 0.91              | 0.89              |
| Random Forest            | 1.94  | 1.00              | 0.96              |
| Gradient Boosting        | 1.28  | 1.00              | 0.98              |
| Support Vector Regressor| 30.31 | 0.69              | 0.69              |
| XGBoost                  | 0.45  | 1.00              | 0.99              |

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost, LightGBM
- Matplotlib, Seaborn
- Jupyter Notebooks

---

## 🚀 Next Steps

- ✅ Deploy model as a REST API using FastAPI
- 📈 Build interactive dashboard using Streamlit
- 🧠 Add SHAP interpretability for model insights
- 🌐 Host report with GitHub Pages

---

## 📬 Contact

For questions, feel free to reach out or open an issue.  
Contributions welcome!

---
