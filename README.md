# Fraud_detection-Accredian-assignment

**📌 Problem Statement**

A financial services company aims to proactively detect fraudulent transactions. The challenge is to build a machine learning model that predicts fraud and to extract insights that guide prevention strategies.

The key expectations include:

Cleaning and preparing the dataset (handling missing values, outliers, multicollinearity).

Building and evaluating a fraud detection model.

Explaining variable/feature selection strategy.

Identifying factors that predict fraudulent behavior.

Proposing prevention measures and ways to evaluate their effectiveness.

**📊 Dataset Description**

Format: CSV file

Size: ~6.36M rows × 10 columns

Content: Transaction-level data with features relevant to fraud prediction

Dataset: Fraud.csv

⚠️ Note: Fraud datasets are typically imbalanced, with far fewer fraud cases compared to legitimate transactions.

**🛠️ Project Workflow**

1. Data Cleaning & Preprocessing
   -------------------------------

Handled missing values and outliers.

Encoded categorical variables using Label Encoding.

Checked for multicollinearity and dropped redundant features.

Normalized features for consistent scaling.

2. Exploratory Data Analysis (EDA)
   --------------------------------

Visualized distributions of key variables.

Analyzed fraud vs non-fraud class balance.

Identified patterns that separate fraudulent from normal transactions.

3. Model Development
   ------------------

Train-test split applied.

Baseline models tested for comparison.

XGBoost Classifier chosen for final training (handles imbalance well, strong performance).

4. Model Evaluation
   ------------------

Classification Report generated (Precision, Recall, F1-score).

ROC-AUC Curve plotted to evaluate discriminative ability.

Achieved strong performance on fraud detection with meaningful trade-off between recall (catching frauds) and precision (avoiding false alarms).

5. Feature Importance & Insights
   -------------------------------

Extracted top predictors of fraud from the trained XGBoost model.

Interpreted whether these features make intuitive business sense.

Connected data-driven insights with domain-level fraud prevention strategies.

6. Actionable Recommendations
   ----------------------------

Strengthen monitoring on high-risk transaction features.

Implement anomaly detection systems for real-time flagging.

Introduce adaptive thresholds for suspicious activity.

Regular retraining of models to adapt to evolving fraud patterns.

**📈 Results Snapshot**

Model Used: XGBoost Classifier

Key Metrics: ROC-AUC, F1-score, Precision/Recall

Outcome: Identified important fraud predictors and designed a framework for proactive prevention.

