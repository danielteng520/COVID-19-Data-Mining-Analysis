# COVID-19 Data Mining Analysis

This repository contains the group project for **TDP 3301: Data Mining**. The project involves the analysis and prediction of COVID-19 daily cases in Malaysia using data mining techniques. The analysis is based on the open data provided by the Malaysian Ministry of Health (MOH), covering different states and age groups.

## Project Overview
The goal of this project is to perform exploratory data analysis, identify key features affecting daily COVID-19 cases, and compare the effectiveness of different machine learning models in predicting case counts for selected Malaysian states. The study focuses on four states: **Pahang, Kedah, Johor,** and **Selangor**.

## Dataset
The dataset is sourced from [MOH's GitHub repository](https://github.com/MoH-Malaysia/covid19-public) and contains data on:
- **Daily COVID-19 cases** by state
- **Age group categories** (child, adult, elderly)
- **Vaccination status**
- **Cases imported or local**
  
The dataset includes 19,504 records with 25 attributes, spanning from the beginning of the pandemic through 2023.

## Key Steps and Findings
### 1. Exploratory Data Analysis (EDA)
- Visualizations of active cases, recovered cases, and new case trends across different age groups and states.
- Analysis of new cases over time using line charts for specific states.

### 2. Feature Selection
- Employed **Boruta** and **Recursive Feature Elimination (RFE)** to identify key features for case prediction. The most impactful features include age groups, vaccination status, and specific age brackets (e.g., 0-4, 18-29 years).

### 3. Model Comparison
- **Classification Models**: Compared **Decision Tree** and **K-Nearest Neighbors (KNN)** classifiers. Initial models showed low accuracy, but hyperparameter tuning improved their performance slightly.
- **Regression Models**: Compared **Decision Tree Regressor** and **KNN Regressor**. The KNN regressor performed moderately well for Pahang, while the models struggled with high error rates for Selangor.

## Results
- **States with Strong Correlation**: Pahang and Johor exhibited strong correlations with other states, indicating similar case patterns due to geographic and demographic factors.
- **Feature Importance**: Age groups, active cases, and vaccination status were key features affecting daily case counts.
- **Model Performance**: Regression models provided better predictive accuracy compared to classification models, with lower mean squared error (MSE) values for states like Pahang and Johor.

## Limitations and Future Work
The current models did not achieve high accuracy due to limited features and potential overfitting. Future work could involve exploring additional datasets, refining feature selection techniques, and experimenting with advanced machine learning models to improve predictive performance.

## License
This project is for educational purposes as part of coursework for TDP 3301.
