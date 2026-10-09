# Fish Market Weight Prediction

## Overview
This machine learning project predicts fish weight in grams from physical measurements and fish species using supervised regression algorithms.

## Dataset
The project report describes 159 fish samples across seven species.

Features include:
- Length1, Length2, and Length3
- Height
- Width
- Species

**Target:** Weight (grams)

The report describes the dataset but does not establish a separate dataset file in the uploaded materials. See the notebook for the actual data-loading procedure.

## Models Evaluated
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor

## Methodology
1. Exploratory Data Analysis (EDA)
2. Standard scaling of numerical features
3. One-hot encoding of species
4. 80/20 train-test split
5. Five-fold cross-validation
6. Model evaluation using RMSE, MAE, and R²

## Reported Results

| Model | Test RMSE | Test MAE | Test R² |
|---|---:|---:|---:|
| Linear Regression | 40.89 | 28.64 | 0.985 |
| Gradient Boosting | 48.65 | 34.19 | 0.979 |
| Random Forest | 52.37 | 32.98 | 0.975 |
| Decision Tree | 68.37 | 42.45 | 0.958 |

*Metrics are transcribed from the accompanying report. Verify them against a fresh notebook run before publishing.*

## Repository Structure
- `notebooks/` — Analysis and model training
- `reports/` — Project report
- `requirements.txt` — Python dependencies

## Installation

```bash
pip install -r requirements.txt
```

## Run the Notebook

```bash
jupyter notebook notebooks/Fish_Weight_Regression.ipynb
```

Run the cells in order.

## Future Improvements
- Collect more fish samples.
- Test XGBoost or neural networks.
- Use SHAP for model explainability.
- Investigate errors for heavier fish.

## Author
Temesgen Bahlbi
