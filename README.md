# Missing Value Imputation Methods (I)

by Aya Tamura, 21 July 2024

## Overview

This project demonstrates various methods for imputing missing values in sample datasets. It specifically focuses on student data, including student IDs, grades, and subject scores (Math, Science, and English). The goal is to practice and evaluate different imputation methods and determine the most suitable technique for the given dataset.

## Objectives

1. **Identify Missing Values**: Analyze the dataset to identify any missing values.
2. **Determine Missing Value Type**: Conduct exploratory data analysis to classify the missingness as Missing Completely At Random (MCAR), Missing At Random (MAR), or Missing Not At Random (MNAR).
3. **Apply Imputation Methods**: Implement various imputation techniques such as mean, median, mode, K-Nearest Neighbors (KNN), and machine learning models.
4. **Evaluate and Discuss**: Discuss the effectiveness of the chosen imputation method for the dataset.

## Dataset

The dataset contains the following columns:
- `StudentID`: Unique identifier for each student.
- `Grade`: Student's grade level.
- `Math`: Scores in Mathematics.
- `Science`: Scores in Science.
- `English`: Scores in English.

The dataset is a sample of 50 students with some missing values in the subject scores.

## Installation

To run this project, you need to install the following Python libraries. You can do this using `pip`:

```bash
pip install missingno pandas numpy matplotlib seaborn scikit-learn
```
ß
## Usage

1. **Load the Dataset**: The sample dataset is created within the script for practice.
2. **Identify Missing Values**:
   - Load and inspect the dataset.
   - Check the percentage of missing values.
3. **Analyze Missing Value Patterns**:
   - Visualize missing values and their correlation with other variables.
   - Determine if the missingness is MCAR, MAR, or MNAR.
4. **Imputation**:
   - Apply mean imputation by grade to replace missing values.
5. **Evaluate**:
   - Discuss the appropriateness of the chosen imputation method based on the analysis.


## Discussion

Mean imputation is chosen for this dataset because:
- Missing values are determined to be Missing Completely At Random (MCAR).
- The dataset does not exhibit extreme values or outliers.
- Imputing based on the mean by grade preserves the statistical properties and accounts for grade-level variations.

## END

