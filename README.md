# Credit Card Fraud Detection using Decision Tree and SVM

This project applies **Decision Tree** and **Support Vector Machine (SVM)** classifiers to detect fraudulent credit card transactions.  
The goal is to build predictive models that can separate legitimate transactions from fraudulent ones effectively.

## 📊 Dataset
The dataset includes anonymized credit card transaction records with features derived from PCA transformations and a binary target variable:
- `0` → Legitimate transaction
- `1` → Fraudulent transaction

## 🚀 Features
- Data preprocessing and handling class imbalance
- Exploratory Data Analysis (EDA)
- Training classification models (Decision Tree & SVM)
- Evaluating and comparing model performance
- Discussion of results and potential improvements

## 🛠️ Requirements
Install the following dependencies:

```bash
pip install pandas numpy matplotlib scikit-learn
```

## ▶️ Usage
Run the Jupyter notebook:

```bash
jupyter notebook Credit_Card_Fraud_Detection_with_DecisionTree_and_SVM.ipynb
```

## 📈 Results
- Decision Tree provides interpretability but may overfit.  
- SVM generalizes better in many cases, particularly with imbalanced datasets.  
- Handling imbalance is crucial for reliable fraud detection.

## 🔮 Future Improvements
- Use ensemble models (Random Forest, XGBoost, LightGBM).  
- Apply resampling techniques (SMOTE, undersampling).  
- Experiment with deep learning models for fraud detection.
