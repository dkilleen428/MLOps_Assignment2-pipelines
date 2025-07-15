# Assignment 2: ML Experiments with Feature Store and Pipeline

**Author:** dkilleen428  
**Platform:** Databricks (Azure)  

## Assignment Instructions

This project is to design a Feature Store with an ML Pipeline using the `athletes.csv` dataset.

**Requirements:**

- Load and explore the data
- Setup an ML pipeline in any MLOps platform of your choice (Databricks used here)
- Use a feature store with the ML Pipeline
- Create two different versions of features
- Train the same algorithm on both versions (without AutoML)
- Use two different sets of hyperparameters (4 total experiments)
- Compare experiments:
  - Quantitatively (model metrics)
  - Qualitatively (plots)
  - Carbon emissions for each run

##  Pipeline Overview

- **Data:** `athletes.csv` (personal details and performance metrics)
- **Features:**
  - **Version 1:** `height`, `weight`, `age`
  - **Version 2:** `height`, `weight`, `age`, and calculated `BMI`
- **Model:** `RandomForestClassifier`
- **Hyperparameters tested:** `n_estimators = 100`, `200`
- **Total Experiments:** 4

Each run was tracked for performance and carbon emissions, using Databricks MLflow and experiment logging tools.

## ChatGPT Use

This project was completed on Azure Databricks with support from:
- **ChatGPT** for troubleshooting feature store issues, cluster setup, GitHub integration, and workflow structuring.


## Files

- `Assignment2.ipynb`: Contains full pipeline code, experiments, and logging
- `README.md`: Overview of the project and assignment requirements
- `athletes.csv`: Data used for the project

