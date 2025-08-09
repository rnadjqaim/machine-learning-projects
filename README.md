# Sleep Health and Lifestyle Analysis

## Overview

This project analyzes the relationship between lifestyle factors (such as stress level, physical activity, and sleep duration) and job-related factors (like occupation) on the quality of sleep.
The goal is to build and evaluate machine learning models that can predict sleep quality based on these features.

## Dataset

**Name:** Sleep Health and Lifestyle Dataset
**Source:** [Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)

## Problem Statement

The objective is to identify patterns and predictors that influence sleep quality. Poor sleep impacts mental and physical health, productivity, and overall well-being.
By understanding these factors, individuals and organizations can take informed actions to improve sleep habits.

**Type of Problem:** Classification
**Target Variable:** `Quality of Sleep`
**Metrics Used:** Accuracy and F1-Score

## Project Steps

1. **Data Loading and Understanding**

   * Loaded dataset and explored structure, missing values, and target distribution.

2. **Data Preprocessing**

   * Encoded categorical variables.
   * Scaled numerical features.
   * Split dataset into Train, Validation, and Test sets.

3. **Exploratory Data Analysis (EDA)**

   * Visualized target distribution.
   * Examined correlations.
   * Detected class imbalance.
   * Identified outliers.

4. **Feature Engineering**

   * Added derived features:

     * Age Group
     * High Stress Indicator
     * Sleep Efficiency

5. **Model Training**

   * Trained and evaluated 5 models:

     * Logistic Regression
     * Decision Tree
     * Random Forest
     * Gradient Boosting
     * Support Vector Machine
   * Selected the best model based on validation F1-score.

6. **Hyperparameter Tuning**

   * Applied `RandomizedSearchCV` on Random Forest for optimal parameters.

7. **Final Evaluation**

   * Assessed the tuned model on the test set using Accuracy, F1-score, Classification Report, and Confusion Matrix.
   * Plotted feature importance.

## Best Model

* **Model:** Random Forest Classifier
* **Performance:** Achieved perfect Accuracy and F1-score on validation and test sets.

## Requirements

* Python 3.x
* pandas
* numpy
* scikit-learn
* matplotlib
* seaborn

## How to Run

1. Clone the repository or download the notebook.
2. Install the required dependencies:

   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Run the notebook step by step.

## Results

The project successfully identified key lifestyle and occupational factors that impact sleep quality, with the Random Forest model providing the best predictive performance.

---

Do you want me to also make a **shorter, GitHub-friendly README.md** version that’s more concise? That would make it perfect for a public repo.
