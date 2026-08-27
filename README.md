# Fugacity 2026 — Machine Learning Hackathon

> End-to-end machine learning workflow for predicting overall reactor yield from chemical-process features.

**Competition:** Fugacity 2026 ML Hackathon
**Institution:** Indian Institute of Technology Kharagpur
**Task:** Regression — Predict `overall_yield`

---

## 🏆 Competition Result

| Metric | Result |
|---|---:|
| Final Rank | **154 / 374 valid submissions** |
| Competition RMSE | **18.8299** |
| MAE | **11.4404** |
| R² | **0.7272** |

The solution was developed through iterative validation, feature engineering, model comparison, feature selection, ensemble experimentation, and leaderboard-oriented optimization.

---

## 🎯 Objective

The objective of the Fugacity 2026 ML Hackathon was to develop a machine learning model capable of predicting **overall reactor yield** from chemical-process features.

The project followed an end-to-end machine learning workflow, beginning with exploratory data analysis and progressing through feature engineering, baseline modeling, hyperparameter tuning, boosting models, feature selection, explainability, ensemble modeling, and final submission generation.

The primary focus was on systematic experimentation and improving generalization rather than optimizing a single model in isolation.

---

## 🔬 Machine Learning Workflow

```
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
Leaderboard Optimization
   │
   ▼
Physics-Informed Experiments
   │
   ▼
Final Model
   │
   ▼
Competition Submission
```

---

## 🧪 Project Development

### 1. Exploratory Data Analysis

The first stage focused on understanding the dataset and identifying important patterns.

The analysis included:

- Dataset structure
- Feature distributions
- Target distribution
- Missing-value inspection
- Feature relationships
- Correlation analysis
- Potential outliers
- Initial understanding of the prediction problem

**Notebook:** [`notebooks/01_EDA.ipynb`](notebooks/01_EDA.ipynb)

### 2. Feature Engineering

Feature engineering experiments were performed to improve the representation of the underlying chemical-process relationships and provide useful inputs for downstream models.

**Notebook:** [`notebooks/02_Feature_Engineering.ipynb`](notebooks/02_Feature_Engineering.ipynb)

### 3. Baseline Models

Initial regression models were trained to establish baseline performance and provide reference points for subsequent optimization.

**Notebook:** [`notebooks/03_Baseline_Models.ipynb`](notebooks/03_Baseline_Models.ipynb)
**Results:** [`reports/baseline_results.csv`](reports/baseline_results.csv)

### 4. Model Tuning

Hyperparameter optimization was performed to investigate whether stronger configurations could improve predictive performance.

**Notebook:** [`notebooks/04_Model_Tuning.ipynb`](notebooks/04_Model_Tuning.ipynb)

### 5. Boosting Models

Several powerful tree-based boosting algorithms were explored and tuned, including:

- CatBoost
- XGBoost
- LightGBM

These experiments were used to compare different gradient/tree boosting approaches and identify strong candidate models.

**Notebook:** [`notebooks/05_Boosting_Models_Tuning.ipynb`](notebooks/05_Boosting_Models_Tuning.ipynb)

### 6. Feature Selection & Explainability

Feature-selection experiments were performed to investigate whether a smaller and more informative feature set could improve model performance.

Model interpretation and feature-importance analysis were also used to understand the contribution of important variables.

**Notebook:** [`notebooks/06_Feature_Selection_Explainability.ipynb`](notebooks/06_Feature_Selection_Explainability.ipynb)
**Selected features:** [`models/selected_features.csv`](models/selected_features.csv)

### 7. Model Ensembling

Multiple strong models were combined to investigate whether ensemble predictions could improve generalization compared with individual models.

Different ensemble configurations and weighting strategies were explored.

**Notebook:** [`notebooks/07_Model_Ensembling.ipynb`](notebooks/07_Model_Ensembling.ipynb)

### 8. Final Submission

The final modeling workflow was used to train the selected approach and generate the competition submission.

**Notebook:** [`notebooks/08_Final_Submission.ipynb`](notebooks/08_Final_Submission.ipynb)

> Competition submission files are intentionally excluded from this public repository.

### 9. Leaderboard Optimization

Additional experiments were conducted to investigate model configurations and prediction strategies with the goal of improving leaderboard performance.

**Notebook:** [`notebooks/09_Leaderboard_Optimization.ipynb`](notebooks/09_Leaderboard_Optimization.ipynb)

### 10. Physics-Informed Optimization

Additional domain/physics-oriented experiments were explored to investigate whether chemical-engineering knowledge could provide useful information for predictive modeling.

**Notebook:** [`notebooks/09B_Physics_Optimization.ipynb`](notebooks/09B_Physics_Optimization.ipynb)

---

## 📊 Models Explored

The project evaluated several tree-based regression approaches, including:

- Extra Trees
- CatBoost
- XGBoost
- LightGBM
- Voting ensembles
- Weighted ensemble approaches

Model performance was compared throughout the experimentation process to identify promising approaches for the final competition workflow.

---

## 📈 Experiment Tracking

Experiment results are stored in:

```
reports/
├── baseline_results.csv
└── optimization_results.csv
```

These files provide a compact record of the model benchmarking and optimization experiments conducted during the project.

---

## 📁 Repository Structure

```
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
```

---

## 📓 Notebook Guide

| Notebook | Purpose |
|---|---|
| `01_EDA.ipynb` | Exploratory data analysis and dataset understanding |
| `02_Feature_Engineering.ipynb` | Feature construction and preprocessing |
| `03_Baseline_Models.ipynb` | Initial model benchmarking |
| `04_Model_Tuning.ipynb` | Hyperparameter optimization |
| `05_Boosting_Models_Tuning.ipynb` | Boosting-model experimentation and tuning |
| `06_Feature_Selection_Explainability.ipynb` | Feature selection and model interpretation |
| `07_Model_Ensembling.ipynb` | Ensemble construction and comparison |
| `08_Final_Submission.ipynb` | Final model workflow and submission generation |
| `09_Leaderboard_Optimization.ipynb` | Additional leaderboard-oriented experiments |
| `09B_Physics_Optimization.ipynb` | Physics/domain-informed experiments |

---

## 🛠️ Tech Stack

- Python
- NumPy
- Pandas
- Scikit-learn
- CatBoost
- XGBoost
- LightGBM
- Matplotlib
- Seaborn
- Jupyter Notebook
- Joblib

---

## 💡 Key Takeaways

The project highlighted several practical aspects of machine learning on structured engineering data:

- Model complexity alone does not guarantee better generalization.
- Feature engineering can influence downstream model performance.
- Feature selection can help identify a more useful subset of predictors.
- Different ensemble configurations can produce different validation behavior.
- Local validation performance and hidden-test/leaderboard performance can differ.
- Domain-informed experimentation can provide useful perspectives even when it does not become part of the final model.
- Systematic experimentation and careful validation are important when working with limited data.

---

## 🏁 Final Outcome

The project progressed through a complete machine learning workflow:

**EDA → Feature Engineering → Baselines → Model Tuning → Boosting → Feature Selection → Explainability → Ensembling → Optimization → Final Submission**

### Final Competition Result

- **Rank:** 154 / 374 valid submissions
- **Competition RMSE:** 18.8299
- **MAE:** 11.4404
- **R²:** 0.7272

The repository documents the experimentation journey from initial data analysis through model development, optimization, and final competition submission.

---

## 🔒 Data & Reproducibility

The original competition datasets and generated competition artifacts are intentionally not included in this public repository.

The following are excluded:

- Raw competition datasets
- Processed competition datasets
- Generated submission CSV files
- Serialized `.pkl` / `.joblib` model files
- Local virtual environments
- Local logs and temporary files

This keeps the repository lightweight and avoids redistributing competition data or generated artifacts.

To reproduce the workflow, place the permitted competition datasets in the expected local `data/` directories and execute the notebooks in sequence.

---

## 👤 Author

**Chaathurya T S**
Machine Learning / Data Science

GitHub: [Chaathurya-t](https://github.com/Chaathurya-t)

---

## 📌 Disclaimer

This repository contains the machine learning workflow and experimentation developed for the Fugacity 2026 ML Hackathon.

Competition datasets and submission artifacts are not included in accordance with the repository's data-handling approach.

The reported competition metrics represent the final submitted result and should not be interpreted as a guarantee of reproducibility on unseen datasets outside the competition environment.
