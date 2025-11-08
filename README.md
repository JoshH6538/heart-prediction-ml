# Heart Failure Prediction

**Team Members:** Abigail Diaz, Joshua Hanscom, Andrew Rivera,
**Course:** CS4661 - Data Science / Machine Learning  
**Instructor:** Professor Mohammad Pourhomayoun  
**Date:** November 2025

---

## Introduction

Heart failure is a serious medical condition influenced by a combination of demographic, clinical, and physiological factors. Early prediction of potential heart failure can support proactive care and improve patient outcomes.

In this project, we analyze the **Heart Failure Prediction** dataset to identify factors associated with heart failure and build models capable of predicting patient survival or risk of heart failure.

### Objectives

1. **Classification:** Predict whether a patient is likely to experience heart failure (or survive) based on health attributes.
2. **Clustering:** Use unsupervised learning to identify subgroups of patients with similar risk profiles.
3. **Feature Analysis:** Investigate which features are most strongly associated with heart failure to uncover key risk indicators.

By comparing multiple modeling strategies, we aim to determine which methods provide the most accurate and meaningful insights into heart failure risk.

---

## Dataset Description

The dataset, sourced from [Kaggle - Heart Failure Prediction Dataset](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction), contains **918 unique patient records**, each with **11 features** and a binary target variable `HeartDisease` (1 = yes, 0 = no).

**Features include:**

- Age
- Sex
- ChestPainType
- RestingBP
- Cholesterol
- FastingBS
- RestingECG
- MaxHR
- ExerciseAngina
- Oldpeak
- ST_Slope

The target variable indicates whether the patient has experienced or is at risk of heart failure.

---

## Data Preprocessing

Before model training, the dataset will be cleaned and prepared as follows:

- **Handle missing values** (if any)
- **Scale numerical variables** as required by model type
- **Split data** into training and testing subsets for evaluation consistency

Reusable preprocessing functions may be stored in a shared utility module for consistent data handling across models.

---

## Methods / Models Used

We explore both **supervised** and **unsupervised** learning methods:

### Supervised Models

- **Logistic Regression:** Baseline model to identify features most strongly influencing heart failure risk.
- **Random Forest:** Captures non-linear relationships and provides robust feature importance metrics.
- **Gradient Boosted Trees (GB Trees):** Improves accuracy through sequential learning and weighted updates.

### Unsupervised Learning

- **Clustering (e.g., K-Means):** Used to explore underlying patterns or patient subgroups within the dataset.

Each team member is responsible for training and evaluating 1-2 models, contributing results to a shared repository for comparison.

---

## Results and Evaluation

Model performance will be compared using metrics such as:

- Accuracy
- Precision / Recall
- F1-Score
- ROC-AUC

Visualizations (confusion matrices, ROC curves, feature importance plots) will accompany the results.

> **Status:** Results pending - to be completed after model training and validation.

---

## Discussion

This section will include:

- Comparison of model performance and interpretability
- Key insights from logistic regression coefficients and tree-based feature importances
- Observations from clustering and subgroup analysis
- Limitations due to dataset size, imbalance, or potential bias

---

## Conclusion

We will summarize findings, highlight effective prediction methods, and discuss potential improvements such as:

- Collecting larger or more diverse datasets
- Incorporating additional health metrics
- Applying deep learning or ensemble techniques

---

## Quick Start Guide

This section explains how to set up and run the Heart Failure Prediction project in a clean Python virtual environment across **Windows**, **macOS**, and **Linux**.

---

### Create a Virtual Environment

Create a virtual environment named `.venv` (recommended).  
If you use a different name, be sure to add it to `.gitignore`

#### Windows (PowerShell)

```powershell
cd path\to\project
python -m venv .venv
.venv\Scripts\activate
```

#### macOS / Linux (Bash or Zsh)

```bash
cd path/to/project
python3 -m venv .venv
source .venv/bin/activate
```

---

### Upgrade pip and install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

If you need to install Jupyter manually:

```bash
pip install notebook
```

---

### Launch Jupyter Notebook

```bash
jupyter notebook
```

---

### Note for Git

If your virtual environment is **not** named `.venv`, add the folder name to `.gitignore` to avoid committing large environment files:

```
venv/
myenv/
```

### References

- **Heart Failure Prediction Dataset** - [Kaggle](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
