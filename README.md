# 🎓 Student Performance & Analytics Dashboard

A machine learning and interactive dashboard project designed to analyze student academic habits, evaluate predictive models, and deploy an interactive analytics interface for educational insights.

---

## 📌 Project Overview

This repository features a complete end-to-end Machine Learning pipeline and Streamlit web application focused on classifying and analyzing student performance[cite: 1, 2]. Using a dataset of student academic metrics, habits, and demographics, we train and evaluate multiple models to predict student academic categories (`Average`, `Good`, `Excellent`).

**Logistic Regression** was chosen as the primary model, achieving a top accuracy of **92.50%** and a Macro F1-Score of **0.8965**, outperforming tree-based and ensemble models on this dataset.

---

## 📊 Streamlit Dashboard Features

The dynamic Streamlit dashboard provides a compact interface for real-time exploratory data analysis and student filtering[cite: 1]:

- **Filter Sidebar:** Dynamic filtering by Performance Label, Parent Education Level, and Tutoring Support[cite: 1].
- **Executive KPI Row:** Key aggregated metrics covering Total Students, Avg GPA, Avg Attendance Rate, Daily Study Hours, and Assignment Completion %[cite: 1].
- **Study Hours by Group:** Bar chart displaying daily study habits segmented by performance classification[cite: 1].
- **Parental Education Distribution:** Interactive donut/pie chart detailing parent background distribution[cite: 1].
- **Dual-Axis Comparison:** Visualizing the direct relationship between Average GPA and Attendance Rate across performance groups[cite: 1].
- **Hierarchical Treemap:** Comparative breakdown mapping Parent Education levels to student performance counts[cite: 1].
- **Data Viewer & Download:** Interactive table allowing custom filtering and CSV export[cite: 1].

---

## 🔬 Machine Learning Summary & Results

### Dataset Overview
* **Total Records:** 200 student profiles[cite: 2]
* **Features:** 11 numerical and categorical input features (GPA, Study Hours, Attendance Rate, Class Participation, Parent Education, etc.)[cite: 2]
* **Target Variable:** `Performance_Label` (`Average`, `Good`, `Excellent`)[cite: 2]

### Model Performance Comparison

| Model | Accuracy | Macro F1-Score |
| :--- | :---: | :---: |
| **Logistic Regression (Selected)** | **92.50%**[cite: 2] | **0.8965**[cite: 2] |
| Random Forest | 85.00%[cite: 2] | — |
| CatBoost | 85.00%[cite: 2] | — |
| XGBoost | 85.00%[cite: 2] | — |

### Key Feature Drivers
Based on coefficient magnitude analysis from the Logistic Regression model, the primary drivers of student performance are[cite: 2]:
1. **Previous GPA** (Strongest predictor)[cite: 2]
2. **Study Hours Per Day**[cite: 2]
3. **Attendance Rate (%)**[cite: 2]
4. **Class Participation**[cite: 2]

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
git clone [https://github.com/your-username/student-performance-dashboard.git](https://github.com/your-username/student-performance-dashboard.git)
cd student-performance-dashboard
