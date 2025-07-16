# Credit Risk Prediction – Kaggle: Give Me Some Credit 🏦

This project predicts the likelihood that a person will experience financial distress in the next two years using real-world credit data.

## 🧠 Objective
Build a binary classification model to predict `SeriousDlqin2yrs` (1 = default risk).

## 📂 Dataset
- Source: [Kaggle - Give Me Some Credit](https://www.kaggle.com/c/GiveMeSomeCredit)
- Train: ~150,000 records, 11 features (income, debt ratio, late payments...)

## ⚙️ Tools & Techniques
- Python, Pandas, XGBoost, Scikit-learn, Joblib
- Handled class imbalance using `scale_pos_weight`
- Evaluation: ROC AUC = **0.85959 (private test)**

## 🔍 Key Steps
- Missing value imputation (median)
- Train/test split with stratification
- Train XGBoost model with tuned parameters
- Predict probabilities and create Kaggle submission

## 📊 Results
- Public Score: 0.85554
- Private Score: **0.85959**

## 💡 Learnings
- How to handle imbalanced datasets in credit scoring
- Importance of threshold tuning vs default 0.5
- End-to-end Kaggle pipeline from training to submission

## 🧾 Files
- `train.ipynb`: training pipeline & model saving
- `test.ipynb`: load model and generate `submission.csv`
