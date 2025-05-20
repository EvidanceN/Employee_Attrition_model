# Employee attrition predictive model 

## Table of Contents

- [Aim](#aim)
- [Data source](#data-source)
- [Data preparation](#data-preparation)
- [Model Training](#model-training)
- [Save the  model](#save-the-model)
- [Test the  model](#test-the-model)
- [Results](#results)
- [Recommandations](#recommandations)
  

### Aim

---

To utilize the employee attrition data to understand what causes employee attrition and create a predictive model to predict employees that are likely to leave the company. This model will help companies understand which factors influence employee attrition and what they can do retain valuable employees.

---

### Data source

Kaggle: [Employee Attrition](https://www.kaggle.com/datasets/stealthtechnologies/employee-attrition-dataset?select=train.csv)

### Tools

- Kaggle
- PowerBI - Creating reports

#### Data preparation
1. Data Cleaning.
2.  Exploratory Data Analysis.
3. Feature Engineering.
4. Model Training.
5. Evaluation.
6. Model Saving and Inference.

### Model training
The model was trained the Logistic Regression which is suitable for binary and multi-class classification problems.

```
 Employees_attrition_model=LogisticRegression()
```

### Save the model
save and load the model for future use

```
# Save the model
joblib.dump(Employees_attrition_model, 'Employees_attrition_model.pkl')

# Load the model (for later use)
loaded_model = joblib.load('Employees_attrition_model.pkl')
```

###  Test the Model

use the loded model and new data to make a prediction

```
#Testing using new data
new_data=(24,2,20,0,7500,0,2,0,2,0,0,0,1,1,1,90,0,0,0,0,2)

# changing the input_data to numpy array
new_data_as_numpy_array = np.asarray(new_data)

# reshape the array as we are predicting for one instance
new_data_reshaped = new_data_as_numpy_array.reshape(1,-1)

prediction = loaded_model.predict(new_data_reshaped)
print(prediction)

if (prediction[0] == 0):
  print('The employee will stay in the company')
else:
  print('The employee will leave the company')
```

### Results

An accuracy of 69.68% was achived using the trained model

### Recommandations

To improve the model 
- Tune hyperparameters
- Try different models





