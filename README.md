# Employee attrition predictive model 

## Table of Contents

- [Aim](#aim)
- [Data source](#data-source)
- [Model Training](#model-training)
- [Model Deployment](#model-deployment)
  

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
4. visulize the data
5. prepare the data for model training

### Model training

1. Connect to the Azure ML workspace
2. import the cleaned dataset and split the dataset into test and train data
3. Set up the AutoML experiment and the AutoML configuration
4. Run AutoML
5. Examine the results
6. Save the best model

### Model deployment

1. Set up an Azure Machine Learning environment to deploy the model
2. Downloading	the scoring file
3. Deploying the model






