# Credit Card Fraud Detection using Random Forest

## Dataset
Kaggle Credit Card Fraud Dataset  
Highly imbalanced dataset with fraud cases < 0.2%.

Due to GitHub file size limits, the dataset is not included in this repository.

Dataset Source:  
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

---

## Objective
Detect fraudulent transactions using machine learning while effectively handling class imbalance.

---

## Models Used
- Logistic Regression (Baseline)
- Random Forest (Final Model)
- XGBoost (Experimental Comparison)

---

## Techniques Used
- Stratified Train-Test Split
- Class Weight Balancing
- Stratified K-Fold Cross Validation
- Threshold Tuning
- ROC-AUC Evaluation

---

## Cross Validation
- 5-Fold Stratified Cross Validation  
- Metric: F1-score  
- Mean F1-score: ~0.81  
- Standard Deviation: ~0.06  

---

## Final Model Performance (Test Set)
- Precision (Fraud): ~0.91  
- Recall (Fraud): ~0.68  
- F1-score (Fraud): ~0.78  
- ROC-AUC: ~0.94  

---

## Files
- `fraud_detection.ipynb` → Complete implementation and experiments
- `random_forest_fraud_model.pkl` → Trained Random Forest model
- `xgboost_fraud_model.pkl` → Trained XGBoost model (optional)
- `feature_importance.png` → Feature importance visualization

---

## Conclusion
Random Forest significantly outperformed the baseline model and handled severe class imbalance effectively.  
XGBoost provided comparable performance and was explored as an advanced ensemble method.
