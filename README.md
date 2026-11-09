# 🎓 Student Performance & Analytics Dashboard

A machine learning and interactive dashboard project designed to analyze student academic habits, evaluate predictive models, and deploy an interactive analytics interface for educational insights.

---

## 📌 Project Overview

This repository features a complete end-to-end Machine Learning pipeline and Streamlit web application focused on classifying and analyzing student performance[cite: 1, 2]. Using a dataset of student academic metrics, habits, and demographics, we train and evaluate multiple models to predict student academic categories (`Average`, `Good`, `Excellent`).

**Logistic Regression** was chosen as the primary model, achieving a top accuracy of **92.50%** and a Macro F1-Score of **0.8965**, outperforming tree-based and ensemble models on this dataset.

---

## 📊 Streamlit Dashboard Features

The dynamic Streamlit dashboard provides a compact interface for real-time exploratory data analysis and student filtering:

- **Filter Sidebar:** Dynamic filtering by Performance Label, Parent Education Level, and Tutoring Support.
- **Executive KPI Row:** Key aggregated metrics covering Total Students, Avg GPA, Avg Attendance Rate, Daily Study Hours, and Assignment Completion %.
- **Study Hours by Group:** Bar chart displaying daily study habits segmented by performance classification.
- **Parental Education Distribution:** Interactive donut/pie chart detailing parent background distribution.
- **Dual-Axis Comparison:** Visualizing the direct relationship between Average GPA and Attendance Rate across performance groups.
- **Hierarchical Treemap:** Comparative breakdown mapping Parent Education levels to student performance counts.
- **Data Viewer & Download:** Interactive table allowing custom filtering and CSV export.

---

## 🔬 Machine Learning Summary & Results

### Dataset Overview
* **Total Records:** 200 student profiles
* **Features:** 11 numerical and categorical input features (GPA, Study Hours, Attendance Rate, Class Participation, Parent Education, etc.)
* **Target Variable:** `Performance_Label` (`Average`, `Good`, `Excellent`)

### Model Performance Comparison

| Model | Accuracy | Macro F1-Score |
| :--- | :---: | :---: |
| **Logistic Regression (Selected)** | **92.50%** | **0.8965** |
| Random Forest | 85.00% | — |
| CatBoost | 85.00% | — |
| XGBoost | 85.00% | — |

### Key Feature Drivers
Based on coefficient magnitude analysis from the Logistic Regression model, the primary drivers of student performance are:
1. **Previous GPA** (Strongest predictor)
2. **Study Hours Per Day**
3. **Attendance Rate (%)**
4. **Class Participation**

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.9+[cite: 1, 2]
* **Data Manipulation:** Pandas[cite: 1]
* **Visualizations:** Plotly Express, Plotly Graph Objects[cite: 1]
* **Machine Learning:** Scikit-learn (Logistic Regression, StandardScaler, SimpleImputer)[cite: 2]

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone [https://github.com/ejiro-eyitene/student-performance-dashboard.git](https://github.com/ejiro-eyitene/student-performance-dashboard.git)
cd student-performance-dashboard
