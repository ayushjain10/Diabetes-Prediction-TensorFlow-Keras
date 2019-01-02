# Diabetes-Prediction-TensorFlow-Keras
Building Neural Network for this classification problem using Keras with TensorFlow as backend

Build Convoluted Neural Network with Keras using Python language

Dataset: Pima Indian Diabetes from Kaggle

This is a classification problem where based on the attributes such as Glucose, BloodPressure, SkinThickness, Insulin predict if the person has Diabetes or not.

The important part of the problem is to identify the optimal number of hidden layers and neuron in the neural network.

There was more accuracy with more number of hidden layers and neurons, but that will overfit our model on the training data and may not predict the optimal solution for the test data.

The problem was solved using the below steps :

  1) Read the data set using pandas library API's and used model_selection from sklearn to get training and test data.

  2) Created a sequential model with a input layer, one hidden layer and an output layer.
     We chose sequential model as it creates model layer by layer.
     We used relu and sigmoid activation function which modifies the output based on the function working.

  3) After creating the model, we compiled the model using Adaptive Moment Estimation to tune the parameters in order to            minimise the error.
     For the loss argument, we chose binary cross_entropy as the parameter as it is efficient for classification problem.
  
  4) We fit the model on the neural network using training data and then make predictions for the test data.
  
Observation : Performance of the model reported was only 65%. To further improve the accuracy, we re-created the model using Dropout Regularization. The logic is to drop some of the neurons during model creation.

This technique improved the model accuracy to 74.22%. The main issue is to select the right number of parameters.

In the end, we have created a Neural Network model which can be used to predict whether the person has diabetes or not.

A Convolution Neural Network was created using Keras with Python implementation using TensorFlow as a backend.
