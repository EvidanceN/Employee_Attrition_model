# Employee attrition predictive model using Azure Machine Learning

## Table of Contents

- [Aim](#aim)
- [Data source](#data-source)
- [Explonetary Data Analysis](#explonetary-data-analysis)
- [Results](results)


### Aim

---

To utilize the employee attrition data to understand what causes employee attrition and create a predictive model to predict employees that are likely to leave the company. This model will help companies understand which factors influence employee attrition and what they can do retain valuable employees.

---

### Data source

Kaggle: [Employee Attrition](https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset?select=train.csv)

### Tools

- Azure Machine Learning Studio
- AutoML
- PowerBI - Creating reports

#### Data cleaning
1. Loading the test.csv and train.csv
2. Checking for missing values

```
Employees_train_data.isnull().sum()
```

### Explonetary Data Analysis

### importing the libraries
```
import pandas as pd 
import numpy as np
import seaborn as sb
import seaborn as sns
import matplotlib.pyplot as plt

from sklearn import metrics
from sklearn.preprocessing import LabelEncoder
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score, classification_report
from sklearn.metrics import confusion_matrix, ConfusionMatrixDisplay
```
#### Data cleaning
1.Checked for missing values. There data had no missing values which imply that the is no  need to clean the data

```
Employees_train_data.isnull().sum()
```
#### Data preprocessing
- feature selection
  
```
  columns=['Gender', 'Monthly Income', 'Job Role', 'Work-Life Balance', 'Job Satisfaction', 'Performance Rating', 'Overtime', 'Education Level', 'Marital Status', 'Job Level', 'Company Size',
       'Remote Work', 'Leadership Opportunities', 'Innovation Opportunities', 'Company Reputation', 'Employee Recognition', 'Attrition']
```
### Model training
### Model deployment
### Testing the deployed model




