Bank Term Deposit Prediction using Logistic Regression
📌 Problem Statement

The objective of this project is to build a Logistic Regression model to predict whether a customer will subscribe to a term deposit based on their banking and demographic information.

📂 Dataset Description
Dataset: Bank Marketing Dataset
Records: ~45,000 customers
Features: 17 attributes including:
Age
Job
Marital Status
Education
Balance
Loan information
Target Variable:
y (yes / no → subscription)
⚙️ Methodology
1. Data Loading
Dataset extracted from ZIP file in Google Colab
Correct CSV file (bank-full.csv) selected
Encoding issue resolved using latin1
2. Data Preprocessing
Converted target variable:
yes → 1
no → 0
Applied One-Hot Encoding to categorical features
Removed redundant columns (if any)
3. Feature Scaling
StandardScaler used to normalize feature values
4. Model Building
Algorithm: Logistic Regression
Library: Scikit-learn
Max iterations increased to ensure convergence
5. Model Evaluation
Accuracy Score
Confusion Matrix
Classification Report (Precision, Recall, F1-score)
📊 Results
Model successfully predicts customer subscription behavior
Achieved reasonable accuracy
Performance depends on data distribution and imbalance
🚧 Challenges Faced
Encoding issues (UnicodeDecodeError)
Incorrect file selection due to _MACOSX folder
Handling categorical variables
✅ Conclusion

Logistic Regression proved to be an effective baseline model for this classification task. With proper preprocessing and feature engineering, it provides reliable predictions.

🚀 Future Improvements
Handle class imbalance (SMOTE or class weighting)
Use advanced models (Random Forest, XGBoost)
Feature selection techniques
ROC-AUC analysis
🛠️ Tools & Technologies
Python
Pandas, NumPy
Scikit-learn
Google Colab
