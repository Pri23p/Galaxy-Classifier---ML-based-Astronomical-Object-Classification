
# Galaxy Classification Project

## Overview
Machine learning solution to classify galaxies into three types (ellipticals, spirals, or galactic mergers) using SDSS and Galaxy Zoo data.

## Data Source
**Dataset**: https://drive.google.com/file/d/10xceTuWJM68t_bknjxstW4POigX4ryGj/view?usp=sharing
- 780 galaxies with color indices, eccentricity, and concentration features
- Three classes: ellipticals, spirals, and mergers

## Technique
- **Algorithm**: XGBoost Classifier with Optuna hyperparameter optimization
- **Features**: Color indices (u-g, g-r, r-i, i-z), eccentricity, adaptive moments, concentration ratios
- **Validation**: 80-20 train-test split with accuracy, ROC-AUC, and confusion matrix
- **Optimization**: 300 trial hyperparameter search using Optuna

## Quick Start
```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost optuna
```

1. Download `galaxy_catalogue.npy` from the Google Drive link
2. Open and run `data1.ipynb` Jupyter notebook
3. Model automatically performs feature engineering, training, and evaluation

## Key Features
- Automated feature engineering with color ratios and statistical aggregations
- Multi-class classification with balanced performance across galaxy types
- Comprehensive evaluation including ROC curves and Cohen's kappa
- Interactive visualizations for data exploration and model interpretation

## Files
- `data1.ipynb`: Complete implementation notebook
- `galaxy_catalogue.npy`: Dataset (download required)
- `README.md`: Project documentation

## Author
**Priyanshu Prakash**

## License
MIT License
