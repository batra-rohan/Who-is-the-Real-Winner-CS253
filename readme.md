# Kaggle Contest: Who is the Real Winner?

This repository contains the code for the Kaggle contest: Who is the Real Winner? This contest was conducted as a Python Assignment in the course CS253: Software Development and Operations under Prof. Indranil Saha.

## Objective

This project aimed to develop a machine-learning model to predict the education levels of politicians based on constituency data.

## Introduction

In this project, we aim to predict the education levels of politicians using various features derived from constituency data. This involves data preprocessing, exploratory data analysis (EDA), feature engineering, model training, and evaluation.

## Dataset

The dataset consists of constituency data and includes the following features:
- Candidate Name
- Candidate ID
- Party
- State
- Total Assets
- Total Liabilities
- Constituency Name
- Education Level (Target variable)

## Exploratory Data Analysis

We undertook an extensive EDA to understand the data better and to preprocess it for modelling. Key operations performed during EDA include:
- Converting monetary values in Total Assets and Total Liabilities from English names to numeric values and using their logarithmic values.
- Encoding categorical variables such as Party and State numerically.
- Removing non-informative features like Candidate Name and Candidate ID due to too many unique values and lack of correlation with the target variable.

## Feature Engineering

Several informative features were engineered based on observations from the data:
- Extracting titles such as "Dr." and "Adv." from Candidate Names, which correlate with higher education levels.
- Identifying reserved constituencies by checking for "(SC)" in Constituency Names, which can help predict education trends.

## Model Selection

Various multi-class classification models were tried, including:
- Decision Trees
- Random Forests
- Support Vector Machines (SVM)
- Naive Bayes

After evaluating different models, the Naive Bayes classifier was chosen for the final predictions due to its performance.

## Results

The final model achieved a public leaderboard rank of 15 in a class of over 200 students.
