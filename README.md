# 💳 Credit Card Fraud Detection with Decision Tree & SVM

## 📌 Project Overview
This project demonstrates how to detect fraudulent credit card transactions using two machine learning classifiers:
- **Decision Tree** → interpretable, rule-based learning
- **Support Vector Machine (SVM)** → better generalization, handles imbalance with class weights

We analyze the dataset, visualize key patterns, train the models, and compare their performance.

---

## 🎯 Objectives
- Load and preprocess the dataset  
- Perform Exploratory Data Analysis (EDA)  
- Train classification models (Decision Tree & SVM)  
- Evaluate and compare model performance  
- Discuss results and potential improvements  

---

## 📂 Dataset
- **Source**: [Credit Card Fraud dataset](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMDeveloperSkillsNetwork-ML0101EN-SkillsNetwork/labs/Module%203/data/creditcard.csv)  
- **Shape**: 284,807 transactions × 31 features  
- **Target**: `Class` (0 = non-fraud, 1 = fraud)  
- **Class imbalance**: ~99.8% non-fraud vs ~0.2% fraud  

---

## 🔍 Exploratory Data Analysis (EDA)

### Fraud Class Distribution  
The dataset is extremely imbalanced.  
![Fraud Class Distribution](Fraud%20Class%20Distribution.png)

### Correlation of Features with Fraud  
Horizontal bar plot showing feature correlations with the fraud class.  
![Correlation of Features with Fraud Class](Correlation%20of%20Features%20with%20Fraud%20Class.png)

### Transaction Amount Distribution  
Most transactions are of very small amounts.  
![Transaction Amount Distribution](Transaction%20Amount%20Distribution.png)

### Transaction Amount by Class  
Fraudulent transactions tend to have different distribution patterns.  
![Boxplot of Transaction Amounts by Class](Boxplot%20of%20Transaction%20Amounts%20by%20Class.png)

### Feature Correlation Heatmap  
Visual correlation among all features.  
![Feature Correlation Heatmap](Feature%20Correlation%20Heatmap.png)

---

## ⚙️ Data Preprocessing
- Standardized features with `StandardScaler`  
- Normalized data with `L1` norm  
- Train-test split (70–30)  
- Applied sample weights to balance class distribution  

---

## 🤖 Model Training
- **Decision Tree Classifier** (max_depth=4, with class weights)  
- **Linear SVM** (`LinearSVC`, `class_weight='balanced'`, hinge loss)  

---

## 📊 Model Evaluation

### ROC-AUC Scores
- **Decision Tree**: 0.939  
- **SVM**: 0.986  

---

### Confusion Matrices (Side-by-Side)

<div align="center">

| Decision Tree | SVM |
|--------------|-----|
| ![Decision Tree Evaluation Results](Decision%20Tree%20Evaluation%20Results.png) | ![SVM Evaluation Results](SVM%20Evaluation%20Results.png) |

</div>

---

### Classification Reports

<details>
<summary>📑 Click to expand reports</summary>

**Decision Tree**
markdown
Copy code
           precision    recall  f1-score   support
     0.0       1.00      0.97      0.98     85307
     1.0       0.04      0.88      0.07       136
accuracy                           0.97     85443
macro avg 0.52 0.92 0.53 85443
weighted avg 1.00 0.97 0.98 85443

markdown
Copy code

**SVM**
markdown
Copy code
           precision    recall  f1-score   support
     0.0       1.00      0.83      0.91     85307
     1.0       0.01      0.98      0.02       136
accuracy                           0.83     85443
macro avg 0.50 0.90 0.46 85443
weighted avg 1.00 0.83 0.91 85443

bash
Copy code

</details>
---
## ✅ Key Insights & Conclusion
- Accuracy is misleading due to **class imbalance** → ROC-AUC is a more reliable metric.  
- **Decision Tree**: good interpretability, moderate recall.  
- **SVM**: very high recall (detects almost all frauds), but very poor precision (many false positives).  
- **Best model here**: SVM (higher ROC-AUC), though practical deployment requires balancing recall vs precision.  

---

## 🚀 Future Work
- Explore ensemble models (Random Forest, XGBoost, LightGBM)  
- Use resampling techniques (SMOTE, undersampling, oversampling)  
- Hyperparameter tuning with GridSearch / RandomSearch  
- Try anomaly detection & deep learning methods  

---

## 📸 Visuals
All plots are stored in this repository.  
To add new figures:  
1. Save in PNG format.  
2. Place them in the root folder (or `images/` if you create one).  
3. Reference with:  
```markdown
![Title](images/filename.png)
yaml
Copy code

---

👉 This version will display all your screenshots **inline in the README**, with captions and structure.  

Would you like me to also **make the confusion matrices appear side-by-side** (Decision Tree vs SVM) in
