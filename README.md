# Report

## Overview
The purpose of this analysis is to evaluate the performance of a deep learning model to predict whether a charity application will be successful. The model was trained on a dataset of over 34,000 charity applications, with features such as the application type, affiliation, classification, use case, organization type, income, and requested funding amount. The target variable is a binary variable indicating whether the application was successful.

## Report

### Data Preprocessing

#### What variable(s) are the target(s) for your model? 
* Target variable: IS_SUCCESSFUL

#### What variable(s) are the features for your model?
* Feature variables: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, ASK_AMT

#### What variable(s) should be removed from the input data because they are neither targets nor features?
* Variables removed from the input data: EIN and NAME (non-beneficial ID columns)


### Compiling, Training, and Evaluating the Model


#### How many neurons, layers, and activation functions did you select for your neural network model, and why?

##### Neural network model structure:
* 3 hidden layers with 80, 30, and 27 nodes, respectively
* Output layer with 1 node and a sigmoid activation function

##### Activation functions:
* Rectified linear unit (ReLU) activation function for all hidden layers
* Sigmoid activation function for the output layer

#### Were you able to achieve the target model performance?
Yes, at a satisfactory level.
* Target model performance: Accuracy of 73%

#### What steps did you take in your attempts to increase model performance?
Steps taken to increase model performance:
* Tried different numbers of hidden layers and nodes
* Tried different activation functions
* Tried different optimizers
* Tried regularization techniques


## Summary

The overall results of the deep learning model are satisfactory, with an accuracy of 73%. However, there is still room for improvement. Some additional steps that could be taken to improve the model performance include:

* Collecting more data, especially for rare categories of applications.
* Using a more sophisticated neural network architecture, such as a convolutional neural network (CNN).
* Using transfer learning from a pre-trained model.
Recommendation for a different model

A different model that could be used to solve this classification problem is a support vector machine (SVM). SVMs are a type of machine learning algorithm that can be used for both classification and regression tasks. SVMs work by finding a hyperplane in the feature space that separates the data points into two classes.

SVMs have been shown to be effective for a variety of classification tasks, including predicting the success of charity applications. One advantage of SVMs is that they are relatively insensitive to the dimensionality of the data. This means that SVMs can be used with a large number of features without overfitting the training data.