# Fugacity 2026 — Machine Learning Hackathon

> End-to-end machine learning workflow for predicting overall reactor yield from chemical-process features.

**Competition:** Fugacity 2026 ML Hackathon  
**Institution:** Indian Institute of Technology Kharagpur  
**Task:** Regression — predict `overall_yield`

---

## 🏆 Competition Result

| Metric | Result |
|---|---:|
| Final Rank | **154 / 374 valid submissions** |
| RMSE | **18.8299** |
| MAE | **11.4404** |
| R² | **0.7272** |

The final model was selected through iterative validation, model comparison, feature selection, ensemble experimentation, and leaderboard-oriented optimization.

---

## 🎯 Objective

The goal of the hackathon was to develop a machine learning model capable of predicting **overall reactor yield** from process and chemical-engineering features.

The project focused not only on achieving a strong validation score, but also on understanding the effect of feature engineering, model choice, feature selection, ensembling, and domain-informed experimentation on generalization.

---

## 🔬 Machine Learning Workflow

The project follows a structured end-to-end workflow:

```text
Raw Data
   │
   ▼
Exploratory Data Analysis
   │
   ▼
Feature Engineering
   │
   ▼
Baseline Models
   │
   ▼
Hyperparameter Tuning
   │
   ▼
Boosting Models
   │
   ▼
Feature Selection & Explainability
   │
   ▼
Model Ensembling
   │
   ▼
Leaderboard / Physics-Informed Optimization
   │
   ▼
Final Model
   │
   ▼
Competition Submission
🧪 Experiments

The project evaluated multiple stages of model development.

Baseline Models

Initial experiments established reference performance for tree-based regression models.

Model Tuning

Hyperparameter optimization was performed to investigate whether stronger configurations could improve validation performance.

Boosting Models

Several gradient/tree boosting approaches were explored, including:

CatBoost
XGBoost
LightGBM
Feature Selection

Feature-selection experiments were performed to determine whether a smaller, more informative feature set could improve generalization.

Explainability

Feature importance and model interpretation were used to understand which variables contributed most strongly to predictions.

Ensemble Modeling

Multiple strong learners were combined using voting/weighted-voting strategies.

The optimization experiments compared different ensemble weightings rather than assuming that equal weighting would be optimal.

Domain-Informed Optimization

Additional physics/domain-oriented experiments were explored to investigate whether chemical-engineering knowledge could improve predictive performance.

📊 Model Development

The main models explored during the project included:

Extra Trees
CatBoost
XGBoost
LightGBM
Voting ensembles
Weighted voting ensembles

The final workflow selected the strongest validated approach and used it to generate the competition submission.

📁 Repository Structure
Fugacity-ML-Hackathon/
│
├── models/
│   └── selected_features.csv
│
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Feature_Engineering.ipynb
│   ├── 03_Baseline_Models.ipynb
│   ├── 04_Model_Tuning.ipynb
│   ├── 05_Boosting_Models_Tuning.ipynb
│   ├── 06_Feature_Selection_Explainability.ipynb
│   ├── 07_Model_Ensembling.ipynb
│   ├── 08_Final_Submission.ipynb
│   ├── 09_Leaderboard_Optimization.ipynb
│   └── 09B_Physics_Optimization.ipynb
│
├── reports/
│   ├── baseline_results.csv
│   └── optimization_results.csv
│
├── .gitignore
├── README.md
└── requirements.txt

The original competition datasets, generated submission files, and serialized model artifacts are intentionally excluded from the public repository.

📓 Notebook Guide
Notebook	Purpose
01_EDA	Exploratory analysis and data understanding
02_Feature_Engineering	Feature construction and preprocessing
03_Baseline_Models	Initial model benchmarking
04_Model_Tuning	Hyperparameter optimization
05_Boosting_Models_Tuning	Boosting-model experiments
06_Feature_Selection_Explainability	Feature selection and interpretation
07_Model_Ensembling	Ensemble construction
08_Final_Submission	Final training and submission generation
09_Leaderboard_Optimization	Additional leaderboard-oriented experiments
09B_Physics_Optimization	Domain/physics-informed experiments
📈 Experiment Tracking

Validation results are stored in:

reports/baseline_results.csv
reports/optimization_results.csv

These files provide a compact record of the model-comparison and optimization experiments.

🛡️ Data & Reproducibility

Competition datasets are not included in this repository.

The following are intentionally excluded:

Raw competition datasets
Processed competition datasets
Generated submission CSVs
Serialized .pkl / .joblib model files
Local virtual environments

This keeps the repository lightweight and avoids redistributing competition data.

To reproduce the workflow, place the permitted competition data in the expected local data/ directories and execute the notebooks sequentially.

🛠️ Tech Stack
Python
NumPy
Pandas
Scikit-learn
CatBoost
XGBoost
LightGBM
Matplotlib
Jupyter Notebook
💡 Key Takeaways

One of the main lessons from the project was the difficulty of generalizing from a relatively small dataset.

The experiments demonstrated that:

model complexity alone does not guarantee better generalization;
feature selection can materially affect ensemble performance;
different ensemble weightings can produce different validation behavior;
local cross-validation and hidden-test performance can diverge;
domain-informed experimentation can be useful even when it does not ultimately become the final model.

The project therefore emphasized validation discipline and systematic experimentation rather than simply optimizing a single model configuration.

📚 Project Outcome

This repository documents the complete experimentation journey from exploratory data analysis through model development, feature selection, ensemble optimization, and final competition submission.

The final competition result was:

154 / 374 valid submissions

with a competition RMSE of:

18.8299

👤 Author

Chaathurya T S

Machine Learning / Data Science

GitHub: Chaathurya-t
