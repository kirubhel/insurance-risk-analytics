# 🛡️ Insurance Risk Analytics - B5W3 Challenge

This repository is part of the 10 Academy B5W3 challenge: **"Insurance Risk Prediction"**, where the objective is to explore and model factors influencing insurance premiums using customer data.

## 📁 Repository Structure

insurance-risk-analytics/
│
├── data/
│ ├── raw/ # Original dataset (MachineLearningRating_v3.txt)
│ ├── processed/ # Cleaned and feature-selected dataset
│
├── notebooks/
│ ├── 01_eda.ipynb # Exploratory Data Analysis
│ ├── 02_hypothesis_testing.ipynb # Statistical tests and insights
│ ├── 03_model_training.ipynb # Model training and evaluation
│ 
│
├── reports/
│ ├── Task4_Report.pdf # Final modeling report
│ └── B5W3_NonTechnical.pdf # Non-technical summary and curiosity questions
│
├── dvc.yaml # DVC pipeline (if set up)
├── .dvc/ # DVC configuration
├── .gitignore
├── requirements.txt
└── README.md # You're here

---

## ✅ Tasks Overview

### 🧪 Task 1: Exploratory Data Analysis
- Investigated data quality, nulls, and outliers
- Visualized key distributions and relationships
- Identified correlation between features and insurance premiums

### 🧮 Task 2: DVC Setup
- Initialized DVC and tracked raw dataset
- Command used:
  ```bash
  dvc init
  dvc add data/raw/MachineLearningRating_v3.txt
📊 Task 3: Statistical Hypothesis Testing
Conducted chi-square and ANOVA tests

Key insights:

Gender and VehicleType influence premium

Age group has a statistically significant effect

🤖 Task 4: Modeling & Evaluation
Trained a Random Forest Regressor to predict InsurancePremium

Evaluation Metrics:

RMSE: 46149.18

R² Score: 0.1874

Optional: SHAP explainability explored (dependency conflicts noted)

📎 Non-Technical Summary (B5W3)
Located in reports/B5W3_NonTechnical.pdf:

Use of QFT (Question Formulation Technique)

Demonstrated curiosity-driven learning

Final top 5 inquiry questions included

📌 How to Run
1. Clone and Setup

git clone https://github.com/kirubhel/insurance-risk-analytics.git
cd insurance-risk-analytics
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

2. Launch Notebooks
jupyter notebook


3. DVC Usage (optional)
dvc pull


📈 Dependencies
Key libraries used:

pandas, numpy

matplotlib, seaborn

scikit-learn

shap (optional; version-sensitive)

Install with:

pip install -r requirements.txt


👤 Author
Kirubel Gizaw
GitHub: kirubhel

📄 License
This project is under the MIT License - see the LICENSE file for details.
