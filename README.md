# Predicting-Diabetes-Outcomes

Project Overview

This project was a continuation of my early experiments in machine learning — aimed at predicting whether a person is likely to have diabetes based on key health indicators.

Using the Diabetes dataset from sklearn.datasets, I explored data preprocessing, model training, performance evaluation, and visualization to understand how predictive models can support health-related decision-making.

🎯 Objective

To build a regression model that predicts diabetes progression based on medical factors like age, BMI, blood pressure, and other diagnostic variables.
The goal was to apply the concepts of data cleaning, correlation analysis, model fitting, and evaluation using real-world health data.

🧱 Project Workflow

1️⃣ Data Loading & Understanding

Dataset imported from sklearn.datasets.load_diabetes().

Each record represented a patient with medical attributes such as:

age

sex

bmi

bp

s1–s6 (blood serum measurements)

target (quantitative measure of disease progression).

2️⃣ Exploratory Data Analysis (EDA)

Used pandas and matplotlib for initial data inspection.

Visualized distributions of features to identify outliers and patterns.

Performed correlation analysis to identify the strongest predictors of diabetes progression.

Found that BMI and blood serum features (s5) had the strongest positive correlation with the target variable.

3️⃣ Feature Selection

Selected features with strong correlation to the target:

BMI, BP, and S5.

These were chosen for their higher predictive value and clinical relevance.

4️⃣ Model Building

Implemented Linear Regression using sklearn.linear_model.

Split the data into training (80%) and testing (20%) sets using train_test_split.

Trained the model to learn relationships between features and diabetes progression.

5️⃣ Model Evaluation

Evaluated the model using:

Mean Absolute Error (MAE): 51.98

R² Score: 0.377

The moderate R² score indicated that while the model captured some patterns, more feature engineering and nonlinear models could improve accuracy.

6️⃣ Visualization

Created a scatter plot comparing actual vs predicted values.

Used seaborn.regplot to visualize model fit and error spread.

💡 Key Findings

BMI and blood serum levels (S5) were strong indicators of diabetes progression.

The model was able to explain about 38% of the variance, which is reasonable for a simple linear regression model.

Demonstrated how linear models can reveal relationships in medical datasets — even with limited preprocessing.

🧰 Tools & Libraries

Category	Tools

Language	Python

Environment	Jupyter Notebook

Libraries	Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

Model	Linear Regression

🧠 Lessons Learned

Data preprocessing and feature selection are crucial before modeling.

Linear regression is a good baseline but not always the most accurate — more complex models could capture non-linear patterns.

Interpreting evaluation metrics helped me understand how to measure real model performance beyond accuracy.
