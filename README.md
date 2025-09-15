Credit Card Fraud Detection 🚨💳

📌 Project Overview

This project focuses on detecting fraudulent credit card transactions using Machine Learning techniques. The dataset contains anonymized transaction features with a binary fraud label (fraudulent vs. non-fraudulent).

The goal is to build, evaluate, and compare models that can effectively identify fraud while handling severe class imbalance.

🎯 Objectives

Perform Exploratory Data Analysis (EDA) to understand patterns and class imbalance.

Apply data preprocessing (standardization, normalization, train-test split, class balancing).

Train and compare two machine learning models:

Decision Tree (max depth = 4)

Support Vector Machine (SVM) with class balancing.

Evaluate models on accuracy, precision, recall, and F1-score.

Discuss results and highlight areas for improvement.

🔬 Tools & Technologies

Python (NumPy, Pandas, Matplotlib, Seaborn)

Scikit-learn (DecisionTreeClassifier, SVM, evaluation metrics)

Data Visualization (EDA plots to highlight fraud imbalance)

📊 Key Insights

The dataset is highly imbalanced (fraud cases are very rare).

Decision Tree provided interpretable rules but risked underfitting with shallow depth.

SVM handled class imbalance better, showing improved recall on fraud detection.

Balancing techniques improved detection of minority fraud cases.

🚀 Results

Decision Tree achieved quick training but limited recall.

SVM delivered better fraud detection performance at the cost of higher computation.

Highlighted the importance of class balancing and careful choice of metrics (recall > accuracy).

📌 Future Improvements

Experiment with ensemble methods (Random Forest, XGBoost).

Apply SMOTE/ADASYN for synthetic oversampling.

Use deep learning (ANN, Autoencoders) for anomaly detection.

Optimize hyperparameters with GridSearchCV / RandomSearchCV
