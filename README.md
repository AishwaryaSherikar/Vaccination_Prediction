# Vaccination_Prediction
🩺 Vaccination Prediction (H1N1 & Seasonal Flu)
📌 Project Overview

This project focuses on predicting whether individuals are likely to take H1N1 and Seasonal Flu vaccines using survey-based demographic, behavioral, and opinion data.
The problem is framed as a multi-label classification task, where two independent vaccination outcomes are predicted simultaneously.

The goal is to build reliable machine learning models that can help public health authorities identify groups requiring targeted awareness and intervention programs.

📂 Dataset Description

The dataset consists of anonymized survey responses.

Features include:

Demographic details (age group, education, income, marital status, etc.)

Health conditions and insurance status

Behavioral patterns (mask usage, social distancing, hand washing)

Opinions and risk perceptions about vaccines

Target variables:

h1n1_vaccine

seasonal_vaccine

🛠️ Tech Stack & Libraries

Programming Language: Python

Libraries Used:

NumPy

Pandas

Matplotlib & Seaborn

Scikit-learn

Imbalanced-learn (SMOTE)

🔍 Project Workflow

Data Loading & Basic Checks

Imported datasets and inspected shape, data types, and missing values.

Exploratory Data Analysis (EDA)

Analyzed class imbalance in vaccination targets.

Visualized distributions of key numerical and categorical features.

Identified behavioral and opinion-based trends influencing vaccination.

Data Preprocessing

Handled missing values using appropriate statistical techniques.

Encoded categorical variables into numerical format.

Applied feature scaling to normalize numerical features.

Addressed class imbalance using SMOTE.

Model Building
Implemented and evaluated multiple machine learning models:

Logistic Regression

K-Nearest Neighbors (KNN)

Support Vector Machine (SVM)

Random Forest

Gradient Boosting

Hyperparameter Tuning

Used GridSearchCV to optimize model performance.

Applied cross-validation for reliable evaluation.

Model Evaluation

Accuracy

ROC-AUC Score

Precision, Recall, and F1-score

Model comparison to identify the best-performing approach.

📊 Results & Insights

Ensemble models like Random Forest and Gradient Boosting performed better than linear models.

ROC-AUC proved more informative than accuracy due to class imbalance.

Behavioral and opinion-based features had a stronger influence on vaccination decisions than demographics alone.

The final models achieved approximately 83–84% accuracy with stable cross-validation results.

⚠️ Challenges Faced

Highly imbalanced target classes.

Large number of categorical variables.

Overfitting risk in complex models.

Long training time for SVM with hyperparameter tuning.

Solutions Implemented:

SMOTE for imbalance handling.

Stratified train-test split.

Feature scaling and regularization.

Model comparison instead of relying on a single metric.

📌 Conclusion

This project demonstrates an end-to-end machine learning pipeline for a real-world healthcare classification problem.
The insights generated can help improve vaccine outreach strategies by identifying hesitant or high-risk populations using data-driven methods.

🚀 Future Improvements

Try advanced ensemble techniques like XGBoost or LightGBM.

Perform feature importance and SHAP analysis for interpretability.

Deploy the model using Flask or FastAPI.

Convert the solution into a dashboard for public health monitoring.

📁 Repository Structure
├── data/
│   ├── train.csv
│   └── test.csv
├── Vaccination_Prediction.ipynb
├── README.md


