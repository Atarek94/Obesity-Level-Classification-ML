# Obesity Level Classification: Predictive Modeling of Lifestyle Factors

This repository contains a comprehensive machine learning project aimed at building a classification model to predict an individual’s obesity category. The project leverages the **Obesity Levels dataset**, focusing on the impact of eating habits, physical activity, and various lifestyle factors.

## 📋 Project Overview

The primary objective of this study is to classify individuals into specific obesity categories (e.g., Normal Weight, Overweight, Obesity) based on their daily habits and physical attributes. This project follows a structured data science workflow, including:

- **Exploratory Data Analysis (EDA):** Statistical and visual analysis of features.
- **Data Preprocessing:** Handling categorical encoding and numerical scaling.
- **Model Development:** Training and comparing multiple classification algorithms.
- **Hyperparameter Tuning:** Optimizing model performance using Grid and Random Search.
- **Feature Importance:** Identifying the most influential factors affecting obesity.

## 📊 Dataset Description

The dataset includes 17 attributes related to:
- **Demographics:** Gender, Age, Height, Weight.
- **Eating Habits:** Frequent consumption of high-caloric food (FAVC), Consumption of vegetables (FCVC), Number of main meals (NCP), Consumption of food between meals (CAEC), Consumption of water daily (CH2O), and Consumption of alcohol (CALC).
- **Physical Condition & Lifestyle:** Smoking habit (SMOKE), Calories consumption monitoring (SCC), Physical activity frequency (FAF), Time using technology devices (TUE), and Transportation used (MTRANS).
- **Target Variable:** `NObeyesdad` (Obesity Level).

## 🛠️ Technical Stack

- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy
- **Environment:** Jupyter Notebook / Google Colab

## 🚀 Methodology & Results

### 1. Exploratory Data Analysis
- Performed data cleaning, including duplicate removal and missing value checks.
- Conducted **ANOVA** and **Chi-Square** tests to statistically validate the relationship between predictors and the target variable.
- Visualized distributions using bar charts, histograms, and box plots.

### 2. Preprocessing Pipeline
- Implemented a robust `ColumnTransformer` pipeline.
- **Numerical Features:** Scaled using `StandardScaler`.
- **Categorical Features:** Encoded using `OneHotEncoder`.
- **Target Variable:** Encoded using `LabelEncoder`.

### 3. Model Performance
Four classification models were evaluated. After hyperparameter tuning, the **Gradient Boosting** model emerged as the top performer.

| Model | Weighted F1-Score |
| :--- | :---: |
| Logistic Regression | 0.85 |
| Decision Tree (Tuned) | 0.94 |
| Random Forest (Tuned) | 0.94 |
| **Gradient Boosting (Tuned)** | **0.97** |

### 4. Key Insights (Feature Importance)
The analysis identified the following as the top 5 most influential factors:
1. **Weight** (Primary predictor)
2. **Age**
3. **Height**
4. **Frequency of Vegetable Consumption (FCVC)**
5. **Number of Main Meals (NCP)**

## 📂 Repository Structure

- `Obesity_Level_Classification.ipynb`: The main Jupyter notebook containing all code and analysis.
- `obesity_data.csv`: The dataset used for training and evaluation.
- `README.md`: Project documentation.

## 📝 Conclusion

The project successfully demonstrates that lifestyle factors and physical attributes can predict obesity levels with high accuracy (**97%**). The results highlight that while weight and age are dominant factors, dietary habits like vegetable consumption and meal frequency play a significant role in classification.

---
*Developed as part of a data science portfolio project.*
