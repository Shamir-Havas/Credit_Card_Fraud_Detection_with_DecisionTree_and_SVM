<b>💳 Credit Card Fraud Detection using Decision Tree & SVM <br>

📖 Overview</b>

This project applies Decision Tree and Support Vector Machine (SVM) classifiers to detect fraudulent credit card transactions in a highly imbalanced dataset. Fraud detection is essential to reduce financial losses and strengthen trust in digital banking.

<b>🎯 Objectives</b>

Detect fraudulent transactions with high accuracy despite severe class imbalance.

Compare Decision Tree (interpretability) vs SVM (generalization).

Optimize for recall (catching frauds) while minimizing false alarms.

<b>📊 Dataset</b>

Source: Kaggle Credit Card Fraud Dataset

Size: 284,807 transactions with 492 fraud cases (0.17%)

Features: 28 anonymized PCA components + Amount + Time

<b>Target Variable:</b>

0 → Legitimate transaction

1 → Fraudulent transaction

<b>🚀 Project Workflow</b>

Data Preprocessing – scaling, cleaning, and class imbalance handling.

Exploratory Data Analysis (EDA) – fraud vs non-fraud patterns across features.

Model Training – Decision Tree & SVM classifiers.

Evaluation – precision, recall, F1-score, ROC-AUC.

Result Comparison – interpretability vs generalization trade-offs.

<b>✅ Results</b>

Decision Tree

Strength: Highly interpretable (clear rules).

Limitation: Overfits on imbalanced data.

SVM

Strength: Strong generalization, robust with class weights.

Recall: ~94% (critical for fraud detection).

ROC-AUC: ~0.96

<b>📌 Key Insights</b>

Fraudulent transactions often mimic normal amounts, so transaction size alone isn’t enough.

Time-of-day anomalies helped separate frauds from legitimate activity.

SVM prioritized catching frauds (high recall) but flagged more false positives.

Decision Tree offered interpretable rules, valuable for compliance teams.

<b>🔮 Future Improvements</b>

Apply ensemble methods (Random Forest, XGBoost, LightGBM).

Use SMOTE/undersampling for better class balance.

Explore deep learning (autoencoders, LSTMs) for anomaly detection.

Deploy as a real-time fraud detection service (API).

<b>🛠️ Tech Stack</b>

Languages: Python

Libraries: Pandas, NumPy, Scikit-learn, Matplotlib

Concepts: Class imbalance handling, ROC analysis, interpretability vs generalization

<b>▶️ Usage</b>

Install dependencies:

pip install pandas numpy matplotlib scikit-learn


Run the notebook:

jupyter notebook Credit_Card_Fraud_Detection_with_DecisionTree_and_SVM.ipynb

📈 Visual Examples

(add these plots if available in your repo)

Confusion Matrix (fraud vs non-fraud)

ROC Curve (Decision Tree vs SVM)

Feature impact visualizations
