# student-career-prediction
A machine learning project exploring student placement prediction and starting salary prediction using the Student Career Success &amp; Placement Prediction Dataset.
------
This project explores two machine learning tasks:
### 1. Classification - Placement Prediction

The goal was to predict whether a student would be placed or not placed.

Three Logistic Regression models were compared:

- Model 1 - Top 5 numerical features
- Model 2 - All numerical features
- Model 3 - Numerical + categorical features

### Results

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Model 1 | 0.8187 | 0.8415 | 0.9460 | 0.8907 |
| Model 2 | 0.8182 | 0.8416 | 0.9451 | 0.8903 |
| Model 3 | 0.8189 | 0.8418 | 0.9458 | 0.8908 |

The results showed that adding more features did not significantly improve the performance compared to using a smaller set of relevant numerical features.

### Most influential features

Some of the most influential features included:

- Employability Score
- Interview Score
- Programming Skill
- Internships
<img width="1093" height="547" alt="image" src="https://github.com/user-attachments/assets/5e1bd0f2-306f-42c8-a9f9-b660ac6ef3d2" />

## 2. Regression - Starting Salary Prediction

The second task was to predict the starting salary of placed students.

Students with `Placement_Status = Not Placed` were excluded because their starting salary was equal to 0.

A Linear Regression model was trained using numerical and categorical features.

### Results

| Metric | Score |
|---|---:|
| MAE | 10,627 USD |
| RMSE | 12,526 USD |
| R² | 0.139 |

The Linear Regression model did not perform well for predicting starting salaries in this dataset.



