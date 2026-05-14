👥 HR Attrition Analysis

A complete end-to-end Data Analytics & Machine Learning project to predict and understand employee attrition using Python, Scikit-learn, and Power BI.

Show Image
Show Image
Show Image
Show Image

📌 Overview
Employee attrition is one of the most costly challenges for organizations. This project analyzes IBM's HR dataset of 1,470 employees to uncover the key factors driving attrition and builds a Random Forest ML model to predict which employees are at risk of leaving.

🖥️ Power BI Dashboard
Show Image
Show Image
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
PropertyDetailsSourceKaggle — IBM HR Analytics Employee Attrition DatasetSize1,470 employees × 35 featuresTarget VariableAttrition (Yes / No)Attrition Rate16.1% (237 out of 1,470 employees left)

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

SplitEmployeesTraining set (80%)1,176 employeesTesting set (20%)294 employees

Stratified split used to maintain the same 16% attrition ratio in both sets.


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
