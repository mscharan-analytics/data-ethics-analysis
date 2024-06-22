# COMPASS Data Fairness Analysis

## Project Overview

This project analyzes the COMPAS (Correctional Offender Management Profiling for Alternative Sanctions) dataset to assess fairness in criminal risk assessment across different demographic groups, particularly focusing on racial disparities.

## Table of Contents

1. [Data Import](#data-import)
2. [Exploratory Data Analysis](#exploratory-data-analysis)
3. [Fairness Analysis](#fairness-analysis)
4. [Key Insights](#key-insights)

## Data Import

The project uses the COMPAS dataset, which includes information about criminal defendants and their predicted recidivism risk. The data is loaded from a CSV file named 'compas-scores-two-years.csv'.

## Exploratory Data Analysis

The EDA includes:
- Age distribution analysis
- Race distribution analysis
- Correlation heatmap of numeric variables
- Decile score distribution
- Recidivism rates by race

## Fairness Analysis

The fairness analysis focuses on two main rules:

1. Assessing the fairness of prior count classifications between African-American and Caucasian defendants.
2. Evaluating conviction rates among different racial groups for recidivism within two years.

The analysis includes:
- Confusion matrices for high-risk classifications
- True Positive Rate (TPR) comparisons between racial groups

## Key Insights

- There are significant differences in recidivism rates and risk assessments across racial groups.
- The COMPAS model shows disparities in its performance between African-American and Caucasian defendants.
- The analysis reveals potential biases in the criminal risk assessment system that warrant further investigation and potential reforms.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn

## Usage

1. Ensure all required libraries are installed.
2. Load the COMPAS dataset ('compas-scores-two-years.csv') into the same directory as the script.
3. Run the Jupyter notebook or Python script to perform the analysis.

## Future Work

- Incorporate more advanced fairness metrics
- Analyze intersectionality of race with other demographic factors
- Develop recommendations for improving fairness in criminal risk assessment
