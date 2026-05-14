# Telecom Churn Classification — KNN vs Decision Tree

**WGU MSDA D209 | Jared Medlin | September 2024**

## Overview

Two supervised classification models built to predict customer churn 
from telecom customer data, using K-Nearest Neighbors (Task 1) and 
a Decision Tree (Task 2), applied to the same dataset and feature set.

## Research Questions

- **Task 1:** Which factors are most indicative of churn? (KNN)
- **Task 2:** Can customer churn be predicted by a decision tree?

## Results

| Model | Accuracy | AUC |
|-------|----------|-----|
| K-Nearest Neighbors (k=14) | 85.1% | 0.872 |
| Decision Tree (max depth=5) | 83.0% | — |

Both models significantly outperform baseline random classification. 
KNN edges out the decision tree on accuracy; the decision tree is 
more interpretable but more prone to overfitting on new data.

## Features Used

Bandwidth_GB_Year, Income, Contacts, Yearly_equip_failure,
Outage_sec_perweek, InternetService, Techie, OnlineSecurity,
Port_modem, StreamingMovies, StreamingTV

**Target variable:** Churn (binary)

## Tools & Methods

- **Language:** Python 3 (Jupyter Notebook)
- **Libraries:** pandas, numpy, scikit-learn, matplotlib, seaborn
- **Techniques:** KNN classification, GridSearchCV for optimal k and 
  max depth, decision tree classification, ROC/AUC scoring, 
  one-hot encoding, min-max normalization

## Repository Contents

| File | Description |
|------|-------------|
| `JaredMedlinD209Task1-2.pdf` | Task 1 written report (KNN) |
| `JaredMedlinD209Task2-2.pdf` | Task 2 written report (Decision Tree) |
| `D209-2.ipynb` | KNN classification notebook |
| `JaredMedlinD209Task2-2.ipynb` | Decision Tree classification notebook |
| `Raw Data/` | telecom customer dataset |  
| `Finished Data/` | Cleaned telecom customer dataset |
