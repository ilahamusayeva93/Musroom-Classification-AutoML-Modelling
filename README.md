# Mushroom Classification with AutoML Modelling

## Overview

This R Notebook focuses on mushroom classification using AutoML modelling with the H2O library. The analysis covers required libraries, data loading, exploration, preprocessing, modelling, model evaluation, and checking for overfitting.

## Script Details

### 1. Required Libraries

- **Libraries:** The script begins by loading necessary R libraries, including `tidyverse`, `data.table`, `h2o`, and others.

### 2. Data Loading

- **Dataset:** The dataset "mushrooms.csv" is loaded using the `fread` function from the `data.table` library.

- **Data Skimming:** Basic statistics and information about the dataset are provided using the `skim` function.

### 3. Data Exploration

- **Column Renaming:** Columns are renamed to replace spaces, hyphens, and slashes.

- **Exploration:** Initial exploration involves viewing the head of the dataset, column names, and opening the dataset in the RStudio Viewer.

### 4. Data Preprocessing

- **Missing Values:** The total count of missing values is calculated and displayed.

- **Categorical Variable Handling:** Categorical variables are identified and converted to factors.

### 5. Modelling

- **H2O Initialization:** The H2O library is initialized for AutoML modelling.

- **Data Splitting:** The data is split into training and testing sets.

- **AutoML Model:** An AutoML model is trained using the `h2o.automl` function with a stopping metric of AUC.

### 6. Model Evaluation

- **Leaderboard:** The leaderboard of the AutoML model is displayed.

- **Prediction:** The test set is used for making predictions, and a threshold is determined based on the F1 score.

- **Metrics and ROC Curve:** Model performance metrics such as precision, recall, true positive rate, false positive rate, and the ROC curve are visualized.

### 7. Check Overfitting

- **AUC Scores:** AUC scores for training, testing, and cross-validation are calculated and displayed.

## Dataset Information

### Description

The dataset includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms. The classes are categorized as edible (e) or poisonous (p).

### Data Dictionary

- A detailed data dictionary is provided, including classes, cap shape, cap surface, cap color, bruises, odor, gill attachment, gill spacing, gill size, gill color, and more.

## How to Use

1. Ensure you have R installed along with the required libraries listed at the beginning of the script.

2. Place the "mushrooms.csv" dataset in the same directory as the notebook.

3. Run the script in an R environment, considering any specific package dependencies.

## Author

- **Author:** Ilaha Musayeva
- **Date:** 11/04/2023


