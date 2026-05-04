# Student Academic Performance Analysis

## Team Name
Studious

## Team Members
- George Khalil  
- Jay Ma  
- Thaneesha Singh  
- Xueyan Xian  

---

## 📊 Project Overview
This project analyzes factors that influence student academic performance using exploratory data analysis (EDA) and machine learning models.

The goal is to understand which features (such as attendance, study time, and resources) most strongly impact exam scores and to build models that can predict student performance.

The target variable in this project is **Exam_Score**, which we aim to predict using various student-related features.

---

## 📁 Dataset
**Student Academic Performance Dataset**

Source:  
https://www.kaggle.com/datasets/ayeshasiddiqa123/student-perfirmance

File used: `data/StudentPerformanceFactors.csv`

---

## 🔍 What We Did

### 1. Data Exploration (EDA)
- Checked dataset structure and data types
- Handled missing values using mode (for categorical features)
- Generated summary statistics
- Created:
  - Correlation heatmap
  - Scatterplots (numeric features vs Exam Score)
  - Boxplots (categorical features vs Exam Score)

---

### 2. Feature Insights
Key findings:
- **Attendance** and **Hours_Studied** have the strongest positive relationship with exam scores
- Other variables like tutoring and previous scores have weaker influence
- Some categorical factors (like motivation and teacher quality) show moderate effects

---

### 3. Models Used
We trained and compared three models:

- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

---

### 4. Model Performance

| Model              | RMSE | R² Score |
|-------------------|------|---------|
| Linear Regression | ~1.80 | ~0.77 |
| Gradient Boosting | ~1.95 | ~0.73 |
| Random Forest     | ~2.23 | ~0.65 |

---

## 📈 Results
- **Linear Regression performed the best overall**
- More complex models did not significantly improve performance
- This suggests the relationships in the dataset are mostly linear

---

## 📂 Project Structure

```text
studious-studentperformance-education/
│
├── data/
│   └── StudentPerformanceFactors.csv
│
├── notebooks/
│   └── Project_Assignment_02.ipynb
│
├── README.md
└── .gitignore
```


---

## 🚀 How to Run

1. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

2. Open the notebook:

```text
notebooks/Project_Assignment_02.ipynb
```

3. Run all cells

---

## 📌 Key Takeaway
Simple features like attendance and study time are strong predictors of academic success, and simple models can perform just as well as more complex ones for this dataset.