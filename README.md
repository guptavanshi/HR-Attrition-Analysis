👥 HR Employee Attrition Analysis & Prediction
Show Image
Show Image
Show Image
Show Image
Show Image

An end-to-end HR analytics project analysing why employees leave IBM, built a Machine Learning model with 83.3% accuracy to predict attrition, and created an interactive Power BI dashboard with actionable retention recommendations.


📌 Business Problem
Employee attrition costs companies 6–9 months of an employee's salary in recruitment and training costs. IBM's HR team needs to:

Understand why employees are leaving
Identify which employees are at highest risk of leaving
Take proactive action before losing valuable talent

This project answers all these questions using Python EDA, Machine Learning, and Power BI.

🎯 Key Business Insights
#InsightBusiness Recommendation1Sales dept has 40%+ attrition rate — highest of all departmentsIntroduce performance bonuses & career growth plans2Employees working overtime are 3x more likely to leaveCap overtime hours, hire additional staff3Employees earning below average salary leave mostSalary revision for bottom 20% earners418-25 age group has the highest attrition rateBetter growth opportunities & mentorship programs5First 2 years are the highest risk period for attritionStronger onboarding & buddy programs6Low job satisfaction (score 1) directly correlates with attritionQuarterly satisfaction surveys with action plans

🤖 Machine Learning Model
ModelAccuracyROC-AUC ScoreLogistic Regression~85%~0.75Random Forest ✅83.3%0.82+
Random Forest was selected as the final model because it has a higher ROC-AUC score — meaning it is better at correctly identifying employees who will actually leave, which is the most important metric for HR teams.

📊 Dashboard Preview
Executive Overview
Show Image
Deep Dive Analysis
Show Image
ML Model Insights
Show Image

📈 Python Analysis Charts
Attrition Overview
Show Image
Attrition by Department
Show Image
Attrition by Age Group
Show Image
Monthly Income vs Attrition
Show Image
Overtime & Job Satisfaction vs Attrition
Show Image
Years at Company vs Attrition
Show Image
Correlation Heatmap
Show Image
Model Comparison
Show Image
Confusion Matrix
Show Image
Feature Importance — Top Factors Causing Attrition
Show Image

📁 Project Structure
HR-Attrition-Analysis/
│
├── data/
│   ├── WA_Fn-UseC_-HR-Employee-Attrition.csv   ← Original dataset
│   ├── hr_clean.csv                              ← Cleaned dataset
│   └── feature_importance.csv                   ← ML model output
│
├── images/
│   ├── 1_attrition_overview.png
│   ├── 2_attrition_by_department.png
│   ├── 3_attrition_by_age.png
│   ├── 4_income_vs_attrition.png
│   ├── 5_overtime_satisfaction.png
│   ├── 6_years_vs_attrition.png
│   ├── 7_correlation_heatmap.png
│   ├── 8_model_comparison.png
│   ├── 9_confusion_matrix.png
│   ├── 10_feature_importance.png
│   ├── dashboard_page1.png
│   ├── dashboard_page2.png
│   └── dashboard_page3.png
│
├── notebook/
│   └── hr_attrition_analysis.ipynb              ← Main analysis + ML notebook
│
├── dashboard/
│   └── HR_Attrition_Dashboard.pbix              ← Power BI dashboard
│
└── README.md

🔍 Project Workflow
Raw HR Data (1,470 employees, 35 features)
            ↓
Data Cleaning & Feature Engineering (Pandas)
            ↓
Exploratory Data Analysis (10 Charts)
            ↓
Machine Learning Model (Random Forest)
            ↓
Model Evaluation (Accuracy, ROC-AUC, Confusion Matrix)
            ↓
Interactive Dashboard (Power BI — 3 pages)
            ↓
Business Recommendations

📂 Dataset

Source: Kaggle — IBM HR Analytics Employee Attrition Dataset
Size: 1,470 employees × 35 features
Target variable: Attrition (Yes/No)
Attrition rate: 16.1% (237 out of 1,470 employees left)


🛠️ Tech Stack
ToolPurposePython 3.xCore programmingPandasData cleaning & analysisNumPyNumerical operationsMatplotlibCharts and visualisationsSeabornEnhanced visualisationsScikit-learnMachine Learning modelsPower BIInteractive dashboardJupyter NotebookAnalysis environment

▶️ How to Run
bash# 1. Clone the repository
git clone https://github.com/guptavanshi/HR-Attrition-Analysis.git

# 2. Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# 3. Download dataset from Kaggle and place in data/ folder

# 4. Open the notebook
jupyter notebook notebook/hr_attrition_analysis.ipynb

# 5. Open dashboard
# Open dashboard/HR_Attrition_Dashboard.pbix in Power BI Desktop

📊 ML Model Details
Algorithm: Random Forest Classifier
Why Random Forest?

Handles both numerical and categorical features well
Resistant to overfitting compared to a single decision tree
Provides feature importance scores to explain which factors drive attrition
Works well with imbalanced datasets like this one (16% attrition)

Train/Test Split: 80% training (1,176 employees) / 20% testing (294 employees)
Stratified split used to maintain the same 16% attrition ratio in both sets

🔮 Future Scope

 Handle class imbalance using SMOTE oversampling
 Try XGBoost and Gradient Boosting for higher accuracy
 Build an employee risk score dashboard showing attrition probability per employee
 Deploy as a Streamlit web app where HR can input employee details and get attrition prediction
 Add SHAP values for better model explainability


👩‍💻 About Me
Vanshika Gupta — Final year B.Tech student passionate about Data Analytics, Business Intelligence & Machine Learning.
Skills: Python · Pandas · SQL · Power BI · Scikit-learn · Matplotlib · Seaborn · Excel
📧 Connect with me on LinkedIn | GitHub


⭐ If you found this project useful, consider giving it a star!
