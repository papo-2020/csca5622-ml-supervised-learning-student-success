# CSCA 5622: ML Supervised Learning - Student Success Prediction

Course: CSCA 5622 - Intro to Machine Learning: Supervised Learning  
University: University of Colorado Boulder  
Author: Philipp Adrian Pohlmann (PHPO4876)  
Date: 14 October 2025

## Project Overview

Analysis of 6,607 student records from Kaggle.com to predict exam performance using supervised learning techniques.

## Problem Statement

Universities need to identify at-risk students early but have limited intervention resources. This project builds predictive models to enable data-driven, proactive student support.

## Methodology

- Dataset: 6,607 students × 20 features (behavioral, demographic, school-related)
- Models Tested: 7 supervised learning approaches
  - Linear Regression (baseline)
  - Decision Tree
  - Random Forest (with hyperparameter tuning)
  - Gradient Boosting
  - Support Vector Regression (SVR)
  - Polynomial Regression

## Key Results

- Best Performing Model: Linear Regression (R² = 0.77, RMSE = 1.80)
- Top 3 Predictors:
  - Attendance: ~40% importance
  - Study Hours: ~30% importance
  - Previous Scores: ~10% importance

## Key Finding

Simple models can outperform complex ensemble methods when data follows linear, additive patterns. Attendance and study hours are the best intervention points grad schools have for improving student outcomes.

## Extension: AI-Assisted Learning

Performed an exploratory analysis of a second dataset from Kaggle.com (23,218 students in 109 countries) looking at ChatGPT usage in education / learning. This brief study identified AI tooling usage, perceived learning efficiency, and confidence in AI assisted work with some promising future predictors to complement more traditional behavioral factors such as identified in the primary dataset.

## Files in This Repository

- `student_success.ipynb` - Primary analysis Jupyter notebook with code and visualizations
- `ML_Intro_SL_methods_PohlmannPA.pdf` - Presentation slides for a video presentation
- `README.md` - This file

## Data Sources

Primary Dataset: Student Performance Factors  
- Source: [Kaggle - Student Success Factors and Insights](https://www.kaggle.com/datasets/anassarfraz13/student-success-factors-and-insights)
- Records: 6,607 rows × 20 columns
- License: CC0 Public Domain

Exploratory Dataset: Global Student Perceptions of ChatGPT  
- Source: [Kaggle - Global Student Perceptions of ChatGPT](https://www.kaggle.com/datasets/jocelyndumlao/global-student-perceptions-of-chatgpt)
- Records: 23,218 rows × 174 columns
- License: CC BY-NC 4.0

*Note: I did not include the datasets in the repo because they can be directly downloaded from the sources above to reproduce analysis if needed.*

## Technical Requirements
```
pandas
numpy
matplotlib
seaborn
scikit-learn
```

## How to Reproduce

1. Download the datasets from the Kaggle links above
2. Place CSV / XLSX files in a directory for processing
3. Open `student_success.ipynb` in Jupyter Notebook or JupyterLab
4. Run all cells sequentially

## Video Presentation

Video presentation submitted separately via course portal (15 minutes)
