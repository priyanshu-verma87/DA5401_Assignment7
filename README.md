# Assignment 7: Multi-Class Model Selection using ROC and Precision-Recall Curves

**Name:** Priyanshu Verma  
**Roll no:** CH22B087  
**Date:** 31-10-2025

---

## Project Overview

This repository contains a Jupyter Notebook that implements a pipeline for multi-class land-cover classification using the UCI Landsat Satellite dataset. The objective is to compare multiple classifier families using threshold-sensitive evaluation tools - ROC and Precision-Recall (PRC) curves - adapted to the multi-class setting via a One-vs-Rest (OvR) scheme. The notebook includes code, plots, and concise conceptual explanations.

---

## Files in this Repository

- `DA5401_Assignment_7.ipynb` — main notebook (code, plots, and written answers).  
- `README.md` — this file.  
- `sat.trn` and `sat.tst`  - UCI dataset.

---

## Dataset

**Landsat Satellite (Statlog / satimage)** - multi-class land-cover dataset from the UCI Machine Learning Repository.


## Notebook Structure

The notebook is organized into the following sections:

1. **Introduction** - assignment objectives and evaluation criteria.  
2. **Data Loading & Preprocessing** - download/read dataset, remove the “mixture/all types” label, standardize features, and create a stratified train/test split.  
3. **Model Setup & Training** - instantiate and train required models:
   - K-Nearest Neighbors (KNN)  
   - Decision Tree  
   - DummyClassifier (prior)  
   - Logistic Regression  
   - Gaussian Naive Bayes  
   - Support Vector Classifier (SVC, `probability=True`)  
4. **Baseline Metrics** — compute Overall Accuracy and Weighted F1 on the test set.  
5. **Multi-class ROC (OvR)** — compute per-class ROC, derive macro-average ROC, and plot macro-averaged ROC curves for each model.  
6. **Precision-Recall (OvR)** — compute per-class PRC, derive macro-average PRC, plot macro-averaged PRC curves for each model, and compute Average Precision (AP).  
7. **Model Comparison & Interpretation** — compare model rankings across Weighted F1, Macro AUC, and Macro AP and interpret differences.  
8. **Final Recommendation** — synthesis and recommended model.  
9. **Brownie Points** — RandomForest/XGBoost experiments and an illustrative model with AUC < 0.5.  

Each section pairs runnable code with brief markdown explanations answering the assignment questions.

---

## Requirements & Installation

Recommended Python: **3.8+**

