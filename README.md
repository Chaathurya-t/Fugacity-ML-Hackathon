# Fugacity 2026 — Machine Learning Hackathon

An end-to-end machine learning project developed for the ML Hackathon of Fugacity 2026 at IIT Kharagpur.

## Objective

The objective was to develop a machine learning model for predicting overall reactor yield from process and chemical engineering features.

## Approach

The project followed an end-to-end workflow:

1. Exploratory Data Analysis
2. Feature engineering
3. Baseline model development
4. Model comparison
5. Feature selection
6. Ensemble modeling
7. Weighted ensemble optimization
8. Final model training
9. Competition submission

## Models

Several regression models were evaluated, including:

- Extra Trees
- CatBoost
- XGBoost
- Voting ensembles

The final selected approach used a weighted CatBoost + Extra Trees ensemble.

## Competition Result

**Final Rank:** 154 / 374 valid submissions

**RMSE:** 18.8299

**MAE:** 11.4404

**R²:** 0.7272

## Key Learning

The project highlighted the difficulty of generalizing from a small dataset. The final hidden-test performance differed from local cross-validation performance, demonstrating the importance of robust validation and domain-informed feature engineering.

## Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- CatBoost
- XGBoost
- Matplotlib
- Jupyter Notebook