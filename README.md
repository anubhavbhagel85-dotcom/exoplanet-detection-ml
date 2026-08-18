# 🌌 Exoplanet Detection using NASA Kepler Data

Detecting exoplanets from stellar light curves using Machine Learning.

## What this project does
- Loads real NASA Kepler mission data (5087 stars, 3197 time-step light curves)
- Visualizes planetary transit signals — brightness dips caused by orbiting planets
- Handles extreme class imbalance (37 exoplanets vs 5050 normal stars)
- Builds a Random Forest baseline (ROC-AUC: 0.91)
- Builds a 1D CNN on raw starlight signals (ROC-AUC: 1.00, F1: 1.00)

## Results
| Model | ROC-AUC | F1 Score |
|---|---|---|
| Random Forest | 0.9168 | baseline |
| 1D CNN (improved) | 1.0000 | 1.0000 |

## Tech Stack
Python, TensorFlow, Scikit-learn, NumPy, Pandas, Matplotlib

## Dataset
NASA Kepler Labelled Time Series Data
👉 https://www.kaggle.com/datasets/keplersmachines/kepler-labelled-time-series-data

## Key concepts applied
- 1D Convolutional Neural Networks on time-series astronomical data
- Class imbalance handling (oversampling + class weights)
- Proper evaluation using ROC-AUC and F1 (not just accuracy)
- Astroinformatics — applying ML to real NASA mission data

## Author
Anubhav Bhagel — CSE Student | Astroinformatics enthusiast
