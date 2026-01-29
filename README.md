# Credit Card Fraud Detection (Optimized Random Forest)

## Project Overview
This project focuses on detecting fraudulent credit card transactions using machine learning.
Since fraud data is highly imbalanced, model evaluation prioritizes **Precision, Recall, and F1-score**
instead of accuracy.

An optimized **Random Forest Classifier** is used to ensure fast execution in Google Colab
while maintaining strong fraud detection performance.

---

## Dataset
- **Name:** Credit Card Fraud Dataset
- **Target Column:** `Class`
  - `0` → Non-Fraud
  - `1` → Fraud
- The dataset is highly imbalanced.

---

## Project Steps
1. Load the dataset and analyze fraud vs non-fraud distribution.
2. Remove non-useful identifier columns such as `Time`.
3. Handle missing and infinite values.
4. Split the dataset using stratified sampling.
5. Train a baseline Logistic Regression model.
6. Train an optimized Random Forest classifier.
7. Evaluate models using precision, recall, and F1-score.
8. Plot feature importance to identify key fraud indicators.
9. Save the best-performing model using `joblib`.

---

## Model Details

### Baseline Model
- Logistic Regression  
- StandardScaler  
- `class_weight = balanced`

### Final Model
- Random Forest Classifier  
- `n_estimators = 50`  
- `max_depth = 10`  
- `min_samples_leaf = 50`  
- `class_weight = balanced`

---

## Deliverables
