# World Bank Gender and Income Analysis

Course Project -- Statistics for Computer Engineering

## Project Overview

This project presents a statistical and machine learning analysis of
global socioeconomic data using World Bank datasets.

The analysis focuses on:

-   Predicting Gender Ratio Class (multi-class classification)
-   Modeling and predicting GNI per capita (PPP)
-   Performing country income clustering
-   Applying statistical hypothesis testing
-   Building a visualization dashboard for economic insights

The project integrates classical statistical methods with modern machine
learning techniques.

------------------------------------------------------------------------

## Objectives

1.  Analyze the relationship between gender labor structure and national
    economic indicators.
2.  Classify countries into Gender Ratio Classes using supervised
    learning models.
3.  Predict GNI per capita using regression models.
4.  Group countries by income level using clustering techniques.
5.  Extract latent structure using PCA and LDA.
6.  Present results through an analytical dashboard.

------------------------------------------------------------------------

## Project Structure

worldbank-gender-income-analysis/
│
├── data/
│   ├── worldbank_gender_2021.csv
│   ├── worldbank_2017_2021.csv
│   ├── countries_regions.xlsx
│
├── notebooks/
│   ├── 01_gender_ratio_workflow.ipynb
│   ├── 02_advanced_models.ipynb
│   ├── 03_clustering.ipynb
│   ├── 04_income_modeling.ipynb
│
├── dashboard/
│   └── worldbank_dashboard.xlsx
│
├── report/
│   └── midterm_project_report.pdf
│
├── README.md
└── requirements.txt

------------------------------------------------------------------------

## Data Sources

-   World Bank socioeconomic indicators\
-   Country regional classification dataset

The datasets were merged using country names to enable regional
analysis.

------------------------------------------------------------------------

## Methods and Techniques

### Data Processing

-   Missing value analysis and removal of high-missing features
-   Median imputation
-   Feature scaling
-   Log transformation for skewed income distribution
-   Feature selection (Variance Threshold, ANOVA F-test)

### Statistical Analysis

-   ANOVA (Analysis of Variance)
-   Chi-square test of independence

### Machine Learning Models

Classification: - Logistic Regression (baseline) - Support Vector
Machine (RBF kernel) - Random Forest Classifier

Regression: - Linear Regression (baseline) - Random Forest Regressor

Unsupervised Learning: - K-Means Clustering - Elbow Method - Silhouette
Score

Dimensionality Reduction: - Principal Component Analysis (PCA) - Linear
Discriminant Analysis (LDA)

------------------------------------------------------------------------

## Key Results

-   Random Forest achieved the best performance for Gender Ratio
    classification.
-   Random Forest Regressor achieved approximately R² ≈ 0.86 for income
    prediction.
-   Countries were grouped into three income clusters: low, middle, and
    high income.
-   Human capital indicators (life expectancy and education enrollment)
    were the strongest predictors of national income.
-   Statistical tests confirmed a significant relationship between
    region and Gender Ratio Class.

------------------------------------------------------------------------

## Tools and Libraries

-   Python
-   Pandas
-   NumPy
-   Scikit-learn
-   Matplotlib
-   Excel (Dashboard Visualization)
