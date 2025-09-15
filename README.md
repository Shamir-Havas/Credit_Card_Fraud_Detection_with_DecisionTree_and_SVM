💳 Credit Card Fraud Detection with Decision Tree & SVM

📖 Overview

This project demonstrates credit card fraud detection using two classification algorithms: Decision Tree and Support Vector Machine (SVM). It focuses on handling highly imbalanced datasets, performing exploratory data analysis (EDA), and comparing model performance using ROC-AUC scores.

Recruiters and reviewers can quickly evaluate your skills in:

Data preprocessing & scaling

Exploratory data analysis with visualizations

Training and evaluating machine learning models

Addressing class imbalance with sample weighting

Communicating results professionally

📊 Dataset

Source: Credit Card Fraud Dataset

Features: Anonymized principal components (V1–V28), Time, and Amount.

Target: Class (1 = fraud, 0 = non-fraud).

Challenge: Imbalanced classes — fraudulent transactions are <1% of total.

🧭 Objectives

Load and preprocess the dataset.

Perform EDA to visualize and understand the data.

Train and evaluate Decision Tree & SVM classifiers.

Compare model performance using ROC-AUC scores.

Discuss findings and potential improvements.

⚙️ Installation

Clone the repository

git clone https://github.com/Shamir-Havas/Credit_Card_Fraud_Detection_with_DecisionTree_and_SVM.git
cd Credit_Card_Fraud_Detection_with_DecisionTree_and_SVM


Install dependencies

pip install -r requirements.txt


Run the notebook or script

jupyter notebook Credit_Card_Fraud_Detection.ipynb
# or
python fraud_detection_with_images.py

🔎 Exploratory Data Analysis (EDA)

Class Imbalance

The dataset is heavily skewed toward non-fraudulent transactions:

Feature Correlation

Correlation between features and fraud occurrence:

🤖 Model Training

Decision Tree Classifier

Algorithm: DecisionTreeClassifier(max_depth=4, random_state=35)

Handling Imbalance: Used compute_sample_weight('balanced').

Advantage: Easy interpretability.

Support Vector Machine (SVM)

Algorithm: LinearSVC(class_weight='balanced', random_state=31, loss='hinge')

Advantage: Strong generalization on imbalanced data.

📈 Model Evaluation

ROC-AUC Scores
Decision Tree ROC-AUC score : 0.939  
SVM ROC-AUC score          : 0.986



✅ Key Takeaways

Fraud detection datasets are highly imbalanced, requiring careful weighting or resampling.

SVM provided superior performance (higher ROC-AUC), while Decision Trees are easier to explain to non-technical stakeholders.

Visualizations (pie chart) provide insight into the data and model performance.

🚀 Future Improvements

Implement ensemble methods (Random Forest, XGBoost) for improved performance.

Use SMOTE or advanced resampling to address imbalance.

Add metrics like Precision-Recall curves for more comprehensive evaluation.

Deploy the model via Flask or Streamlit for real-time fraud detection demos.

Automate hyperparameter tuning using GridSearchCV or Optuna.

📂 Repository Structure
├── Credit_Card_Fraud_Detection.ipynb   # Main notebook  
├── fraud_detection_with_images.py      # Script version with image saving  
├── images/                             # Saved plots for README  
│   ├── class_imbalance.png  
│   ├── feature_correlation.png  
│   └── roc_comparison.png  
├── requirements.txt                    # Dependencies  
└── README.md                           # Project documentation  

🏆 Skills Demonstrated

Python: Pandas, NumPy, Matplotlib, Scikit-learn

Machine Learning: Decision Tree, SVM, handling imbalanced data

Data Visualization: Pie charts, 

Software Engineering: Clean project structure, reproducibility, and documentation
