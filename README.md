

# Binary Prediction of Poisinous Mushroom classification
## Kaggle top 10 Submission Score(90.8 MCC)
RoadMap
- importing dataset
- EDA Analysis
- Data Transformation
- Strategy -- Stratified K-Fold
- Model training (XGboost, logistic, K-Means, SVM)
- Ensembling
- Submission File

## Requirements

Install my-project with npm

```bash
  import pandas as pd
  import numpy as np
  import matplotlib.pyplot as plt
  import seaborn as sns
  
```
    
## Dataset Used: Kaggle Train.csv

![App Screenshot](https://snipboard.io/yKeBXc.jpg)

## EDA Analyses
### No. of unique values
![unique_value_1](https://github.com/user-attachments/assets/d0ab4c44-3737-41c8-8af9-3e8689117a45)
#### Distribution
![unique_values](https://github.com/user-attachments/assets/1e54f85f-08c7-4b5c-9375-9a7c089c0dfe)
### Percentage of Missing values (train)
![missing_values](https://github.com/user-attachments/assets/8b2ec5e6-5d65-4187-83b0-6fbe808597f0)
### Percentage of Missing values (test)
#### Similar pattern found in test dataframe
![test_missing_values](https://github.com/user-attachments/assets/1395d055-dc10-4e7e-9170-dd95cc4f7415)

### Distribution of Target Variable
![distribution_main](https://github.com/user-attachments/assets/7ce03fee-3f3f-46ff-b8ac-75692f2e20aa)

## Model - Xgboost
#### Prediction probability (evaluation phase)
![xgboost](https://github.com/user-attachments/assets/caa31ae5-e3ea-452d-ba36-fc1efaa926ca)

## Model - Random Forrest
#### Prediction probability (evaluation phase)
![random_forrest](https://github.com/user-attachments/assets/19e39339-503a-4d8c-9fe9-e5229917bd98)

## Model - CatBoost
#### Prediction probability (evaluation phase)
![cat_boost](https://github.com/user-attachments/assets/5e694edc-80c9-4d16-bd0b-0535f5bf4684)
### Conclusion - Xgboost tend to have much higher Confidence Level compared to Other Models
### Ensembling results
#### Hard and Soft Voting is analysed before Hill Climb Racing
#### Stratified K-Fold is used during training and Optuna is used for Hyperparam Tuning
![ensembling_r](https://github.com/user-attachments/assets/e9343b86-1b19-4d1d-9d52-053b70abfae7)
#### Submission file is created using Unique id's and Target Variable

