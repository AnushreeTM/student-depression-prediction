🎓 Student Depression Prediction

A machine-learning classification project that predicts whether a student is likely to be experiencing depression, based on academic, lifestyle, and demographic factors. Built end-to-end using the CRISP-DM framework, comparing four models across accuracy and ROC-AUC.

📌 Overview
Goal: Predict student depression (binary classification) to help identify at-risk students early
Dataset: Student Depression Dataset (Kaggle) — 27,901 records · 18 features
Framework: CRISP-DM (Business Understanding → Data Understanding → Data Preparation → Modeling → Evaluation → Deployment)
Best model: Logistic Regression — 84.6% accuracy
🛠️ Tech Stack

Show Image Show Image Show Image Show Image Show Image Show Image Show Image

🔎 Workflow (CRISP-DM)
Business Understanding — framed the problem: predict depression to support early student wellbeing interventions.
Data Understanding — explored 27,901 records across 18 features (age, academic pressure, CGPA, study satisfaction, sleep, financial stress, etc.).
Data Preparation — handled missing values, encoded categorical variables with LabelEncoder, and split into train/test sets.
Exploratory Data Analysis — visualised distributions and relationships between lifestyle/academic factors and depression.
Modeling — trained Logistic Regression, Random Forest, Decision Tree, and XGBoost.
Evaluation — compared models using accuracy, classification reports, confusion matrices, ROC curves, and feature importance.
📊 Results
Model	Accuracy
Logistic Regression	84.6% ⭐
Random Forest	84.1%
XGBoost	84.1%
Decision Tree	78.0%

Logistic Regression delivered the best performance with strong recall (0.90) on the depressed class — important in a screening context, where missing an at-risk student is costlier than a false alarm. ROC-AUC and feature-importance analysis highlighted the strongest predictors of student wellbeing.

🚀 How to Run
bash
git clone https://github.com/AnushreeTM/student-depression-prediction.git
cd student-depression-prediction

pip install pandas numpy scikit-learn xgboost matplotlib seaborn

jupyter notebook Python_code.ipynb
📁 Repository Structure
student-depression-prediction/
├── Python_code.ipynb       # Full CRISP-DM analysis and modelling
├── data/                   # Student Depression Dataset
└── README.md
📈 Key Takeaways
A simple, interpretable model (Logistic Regression) matched or beat more complex ensembles — valuable when the results need to be explained to non-technical stakeholders.
Recall was prioritised over raw accuracy given the sensitive, screening nature of the problem.
Feature-importance analysis surfaced the academic and lifestyle factors most associated with student wellbeing.
