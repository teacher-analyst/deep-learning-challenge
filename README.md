# deep-learning-challenge
This project is part of Module 21 Challenge of the Monash University Data Analytics Bootcamp. 

## Project Description
### Problem
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

### Deliverables
1. Preprocess the data
2. Compile, train and evaluate the Neural Network model using Tensorflow
3. Optimise the model until a target prdictive accuracy of 75% or hight is achieved
4. Write a report on the Neural Network Model

### Technology 
- Tensorflow
- sklearn
- pandas

## Report
### Overview
The purpose of this analysis is to document the optimisation of a neural network model that will accuractely predict if an organisation funded by Alphabet Soup will be successful. 

### Results
Data processing: 
1.	In reference to the python script seen below, the target variable is ‘IS_SUCCESSFUL’ column.
2.	In reference to the python script seen below, the feature variables are ‘APPLICATION’, ‘CLASSIFICATION’ and ‘NAME’ columns.
![image](https://github.com/teacher-analyst/deep-learning-challenge/assets/130710065/1e39a9a2-1170-4ec0-abea-efdaf3ef42bc)
3. The variable removed from the input data is the EIN column
<img width="629" alt="image" src="https://github.com/teacher-analyst/deep-learning-challenge/assets/130710065/08a54bb2-c29b-4368-baa1-cd1b7f4b20e1">

4. Initially, before optimising the model, I had chosen two hidden layers with 8 neurons in the first layer and 5 neurons in the second layer. The two functions used were relu for the hidden layers and sigmoid for the outer layer.
5. I fell short of the target model performance, achieving an accuracy of only 72%. This is an improvement on the initial model which acheived 61% accuracy.
6. When preprocessing the data, I only removed the ‘EIN’ column and left the NAME column to use as a feature, there were three features in total. Then, I increased the number of Epochs from 100 to 150. In the first attempt at model optimisation, I increased the number of features. In the second attempt, I increased the number of neurons in each hidden layer and in the third attempt, I increased the number of hidden layers from two to three. 
  
### Summary 
The only change that seemed to have a significant impact on model performance was the addition of a third feature i.e. NAME. The addition of a feature increased the model accuracy from 61% to 72%. 
