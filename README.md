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
