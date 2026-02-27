# NYU-DS-GA-1007

## Richter's Predictor: Modeling Earthquake Damage

A data science project for NYU DS-GA 1007 that predicts earthquake damage levels to buildings using machine learning. The project uses data from the 2015 Gorkha earthquake in Nepal, sourced from [DrivenData](https://www.drivendata.org/).

## Project Overview

This project solves a binary classification problem: predicting the level of damage to buildings caused by an earthquake based on building location and construction features. The prediction quality is evaluated using [Log-Loss](https://www.kaggle.com/dansbecker/what-is-log-loss).

### Key Features
- Exploratory Data Analysis (EDA) with visualizations
- Feature engineering: log transformations, outlier handling, interaction features, and binning
- Model comparison: XGBoost vs. LightGBM
- Hyperparameter optimization using Optuna (Bayesian optimization)
- Feature importance analysis

### Results
- LightGBM outperformed XGBoost (log-loss: 0.44 vs 0.46)
- Optuna-tuned LightGBM without feature selection achieved the best validation log-loss (~0.43)
- Test set submission scored ~0.42 log-loss on Kaggle (top-10 ranking)

## Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm optuna
```

### Running the Notebook
1. Open `1007_Datathon.ipynb` in Google Colab or Jupyter
2. Update the data file paths to point to your local copies of `train.csv` and `test.csv`
3. Run all cells sequentially

## Project Structure
```
NYU-DS-GA-1007/
├── README.md                 # This file
└── 1007_Datathon.ipynb       # Main analysis notebook
```

## Authors

NYU DS-GA 1007 project team.
