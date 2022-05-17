# Neural_Network_Charity_Analysis
## Overview
This project tried to predict whether applicants will be successful if funded by the Alphabet Soup Co. Alphabet Soup Co. wants to provide funding to companies. However, it needs to know in advance whether it will be successful or not. Money is on the line here, and we would not want it to waste.

For this, I will create a neural network by using Data Manipulation, creating training and testing sets, and finally analyzing the models I have created.

## Results

### Data Processing

I removed the EIN and NAME columns to clean the data since they have no value to the model.
The varibales being considered for my model are as follows: 'STATUS', 'ASK_AMT', 'IS_SUCCESSFUL', 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT'. I dropped "USE_CASE_Other","AFFILIATION_Other" columns.
My Dependent variable is "IS_SUCCESFUL" since we want to try to predict this with high accuracy.

### Compiling, Training, and Evaluating the Model 

Attempt #1

2 Hidden Layers
 30 neurons (Layer1), 0 neurons(Layer2)
Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classification problems like this and relu are for nonlinear datasets.
Removed "USE_CASE_Other","AFFILIATION_Other" columns.

![alt text](https://github.com/harryhua2021/Neural_Network_Charity_Analysis/blob/main/images/Attempt_1.png)

Attempt #2

3 Hidden Layers
80 neurons (Layer1), 30 neurons(Layer2), 15 neurons(Layer3)
Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classification problems like this and relu is for nonlinear datasets.
Removed "USE_CASE_Other","AFFILIATION_Other" columns.

![alt text](https://github.com/harryhua2021/Neural_Network_Charity_Analysis/blob/main/images/Attempt_2.png)

Attempt #3

3 Hidden Layers
80 neurons(Layer1), 35 neurons(Layer2), 10 neurons (Layer3)
Used Relu and Sigmoid Activations Functions since sigmoid is best for binary classification problems like this and relu is for nonlinear datasets.

![alt text](https://github.com/harryhua2021/Neural_Network_Charity_Analysis/blob/main/images/Attempt_3.png)


## Summary
On Average my models kept around 73% accuracy score which is decent considering it was an improvement. My recommendation to improve this model would be to find better features to help explain what determines "IS_SUCCESFUL" such as more in-depth knowledge of the other associates/ firms being funded. At the end of the day, knowledge is power and if we had more in-depth data between all these applications, we can create a better model.
