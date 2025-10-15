# 💻 Laptop Price Forecasting

This project focuses on predicting **laptop prices** based on various hardware specifications and features using multiple regression models.  
The goal was to identify which specifications most influence laptop prices and compare model performances.

---

## 📊 Project Overview

- Performed **data cleaning**, **feature engineering**, and **exploratory data analysis (EDA)**.  
- Built multiple machine learning models to forecast laptop prices.  
- Compared model accuracy using metrics like **R²** and **MAE**.  
- Visualized feature importance and price trends for better interpretability.

---

## 🧩 Dataset

The dataset contains details about laptops, including:
- **Brand**
- **Processor** (Type & Generation)
- **RAM**
- **Storage (SSD & HDD)**
- **Display Type & Resolution**
- **Weight**
- **Operating System**
- **Price**

> The dataset was preprocessed and cleaned before modeling.  

---

## 🧹 Data Preprocessing Steps

- Handled missing values and removed duplicates.  
- Cleaned inconsistent units (RAM in GB, weight in kg, etc.).  
- Converted text-based features into structured, numeric form.  
- Standardized numeric columns using `StandardScaler`.  
- Encoded categorical features using `LabelEncoder`.

---

## 🧠 Feature Engineering

Created new and more meaningful features:
- **Processor Brand** and **Generation** extracted from processor names.  
- **Total Storage** = SSD + HDD.  
- **Display Quality** derived from screen type and resolution.  

These features helped models better understand relationships between specifications and price.

---

## ⚙️ Model Development

Trained and evaluated multiple regression models:

| Model | R² Score | MAE |
|-------|-----------|-----|
| **KNN Regressor** | 0.5546 | 264.38 |
| **Linear Regression** | 0.7381 | 257.93 |
| **Decision Tree Regressor** | 0.7033 | 239.62 |
| **Random Forest Regressor** | 🏆 **0.8781** | 🏆 **160.11** |

> **Random Forest Regressor** performed best overall with the lowest prediction error and highest R² score.

---

## 📈 Key Insights

- **RAM**, **Processor**, and **SSD capacity** are the strongest predictors of price.  
- High-end configurations (more RAM, faster processors, SSD storage) show a sharp rise in prices.  
- Ensemble models like Random Forest provide strong generalization on unseen data.  

---

## 📊 Visualizations

- Correlation heatmaps to explore feature relationships.  
- Scatter plots and pair plots for visual analysis of price distribution.  
- Feature importance plots highlighting key predictors.

---

## 🚀 Results Summary

- Best Model: **Random Forest Regressor**
- R² Score: **0.878**
- MAE: **₹160.11**
- The model captures complex nonlinear relationships effectively.

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**
- **Scikit-learn**
- **Google Colab**

---

## 🔮 Future Work

- Deploy as a **Streamlit web app** for interactive price prediction.  
- Extend dataset with **brand-specific pricing trends**.  
- Try deep learning models (e.g., ANN or Gradient Boosting) for performance comparison.  

---

## 📂 Repository Structure

