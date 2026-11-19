# Mice Protein Classification with PCA

A data science project exploring protein expression data from mice and comparing machine learning models for multiclass classification.

## Project Overview

The dataset contains 1,080 measurements, 77 protein features, and 8 classes. The project compares models using the full feature set and PCA-reduced features.

## Methods

- Preprocessed missing values and standardized features
- Applied PCA to retain at least 95% of the variance, reducing 77 features to about 30 components
- Compared Support Vector Machine (RBF kernel) and Random Forest
- Used 5-fold group cross-validation by mouse to reduce data leakage
- Evaluated models using Accuracy, Macro F1, and Balanced Accuracy

## Results

The SVM model using the full feature set achieved **68.2% accuracy** and **64.3% Macro F1** in grouped cross-validation. PCA reduced the feature dimensions, though it did not improve classification performance in this experiment.

## Tools

Python, pandas, scikit-learn, Matplotlib, and Google Colab

## How to Run

1. Open the notebook in Google Colab.
2. Run the cells from top to bottom.
3. Follow the notebook instructions to load the dataset and reproduce the analysis.

## Dataset

UCI Mice Protein Expression dataset. See the notebook for the dataset source and preprocessing details.
