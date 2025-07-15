# Assignment 2: ML Experiments with Feature Store and Pipeline

**Author:** dkilleen428  
**Platform:** Databricks (Azure)  


## Objective

To build and evaluate a machine learning pipeline using two versions of engineered features with a feature store-like approach, tracking both performance and carbon emissions.


## Experiments

Created two feature sets:

- **Feature Set V1:** `height`, `weight`, `age`
- **Feature Set V2:** `height`, `weight`, `age`, and calculated `BMI`

A simulated binary label was added for classification experiments.


## Pipeline Details

- **Algorithm:** RandomForestClassifier (no AutoML)
- **Hyperparameters tested:** `n_estimators = 100` and `200`
- **4 total runs:**
  - V1 + 100 estimators
  - V1 + 200 estimators
  - V2 + 100 estimators
  - V2 + 200 estimators


## Results

| Feature Version | n_estimators | Accuracy | CO₂ Emissions (kg) |
|-----------------|--------------|----------|---------------------|
| v1              | 100          | 0.5028   | 0.000679            |
| v1              | 200          | 0.5028   | 0.000005            |
| v2              | 100          | 0.4966   | 0.000666            |
| v2              | 200          | 0.4998   | 0.001136            |

