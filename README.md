# Socially-Awkward

# 🧠 Personality Prediction using XGBoost  

This repository contains the code and pipeline for predicting **Personality Types (Extrovert / Introvert)** from structured data using **XGBoost**. The project was built for a Kaggle-style competition with submission in the format:


---

## 📊 Dataset  

- **train.csv** → contains features + `Personality` target column  
- **test.csv** → contains features without `Personality`  
- **Target** →  
  - `0` → Extrovert  
  - `1` → Introvert  

---

## ⚙️ Approach  

1. **Data Preprocessing**
   - Dropped `id` column from training features.
   - Handled class imbalance using `scale_pos_weight` in XGBoost.

2. **Model Selection**
   - Used **XGBoost Classifier** (`XGBClassifier`) for its ability to handle tabular, imbalanced datasets.
   - Performed **RandomizedSearchCV** with Stratified K-Folds for hyperparameter tuning.  

3. **Evaluation Metrics**
   - Accuracy
   - Precision, Recall, F1-score
   - Confusion Matrix
   - Feature Importances  

---

## 🔥 Results  

📈 **Classification Report**  
<img width="856" height="611" alt="image" src="https://github.com/user-attachments/assets/9e6f7241-9bba-441c-9296-f213d9852c02" />


🛠️ Technologies Used

Python 3.11

XGBoost

scikit-learn

Pandas, NumPy

Matplotlib, Seaborn

📈 Feature Importance

The top features influencing the model are visualized using XGBoost’s plot_importance.

🏆 Competition Ready

This pipeline achieved 97.1% accuracy with balanced performance across both classes, making it suitable for Kaggle leaderboard submissions.

👨‍💻 Author:Rohan Singh
📅 Year: 2025
📌 License: MIT
