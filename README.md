> **Project Type:** Course-based machine learning project developed for educational and portfolio purposes.
# Social Media Impact Analysis

## Overview

This project explores the relationship between social media usage, lifestyle factors, and students' mental well-being using exploratory data analysis and machine learning.

The goal is to build a regression model that predicts **Mental Health Index** based on factors such as social media usage, sleep patterns, perceived stress, and demographic characteristics.

---

## Dataset

The dataset contains **4,500 student records** with information including:

- Daily social media usage
- Weekend social media usage
- Primary social media platform
- Sleep duration and sleep quality
- Late-night usage
- Social comparison frequency
- Perceived stress
- Demographic characteristics
- Mental Health Index

The target variable used in this project is:

**Mental_Health_Index**

---

## Project Workflow

The analysis follows an end-to-end machine learning workflow:

1. Data exploration and visualization
2. Train-test split
3. Missing value analysis and preprocessing
4. Feature engineering
5. Categorical variable encoding
6. Feature scaling
7. Model training
8. Cross-validation
9. Hyperparameter tuning
10. Final model evaluation

---

## Models

Three regression approaches were explored:

- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor

Random Forest was also fine-tuned using **GridSearchCV**.

---

## Model Performance

| Model | Training RMSE | Cross-Validation RMSE | Test RMSE |
|---|---:|---:|---:|
| Linear Regression | 5.72 | 5.77 | 5.93 |
| Decision Tree | 0.00 | 8.37 | 8.85 |
| Random Forest | 2.27 | 5.98 | 6.24 |
| Tuned Random Forest | 4.01 | 5.88 | 6.08 |

**Linear Regression** achieved the best generalization performance among the models tested, with a test RMSE of approximately **5.93**.

The Decision Tree achieved nearly zero training error but performed substantially worse on validation and test data, indicating overfitting.

---

## Key Findings

Exploratory analysis suggests that:

- Higher daily social media usage is associated with a lower Mental Health Index.
- Longer sleep duration is associated with a higher Mental Health Index.
- Higher perceived stress is associated with a lower Mental Health Index.
- More complex models did not necessarily outperform the simpler Linear Regression model.

These findings represent **associations in the dataset and should not be interpreted as causal relationships**.

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

Machine learning techniques used include:

- Data preprocessing pipelines
- One-Hot Encoding
- Feature scaling
- Linear Regression
- Decision Tree Regression
- Random Forest Regression
- Cross-Validation
- Grid Search

---

## Repository Structure

```text
Social-Media-Impact-Analysis/
│
├── Dataset---Social_media_impact_on_life.csv
├── social_media_mental_health_analysis.ipynb
└── README.md
