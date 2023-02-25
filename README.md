# Hyperparameters Tuning in Keras using GridSearchCV
In this repository, we demonstrate how to tune hyperparameters of a Keras neural network using GridSearchCV in scikit-learn to get the best performance ever.

### Dataset
We use the Pima Indians Diabetes dataset as an example. This dataset describes the medical records for Pima Indians and whether or not each patient developed diabetes.
The datasets consists of several medical predictor variables and one target variable, Outcome. Predictor variables includes the number of pregnancies the patient has had, their BMI, insulin level, age, and so on.



### Requirements
Python 3.x
Keras
scikit-learn
NumPy

### Tuning the most common hyperparameters of a neural network model using Grid Search 
The script is divided into six parts:

* Tuning Batch Size and Number of Training Epochs
* Tuning Optimization Algorithms/Optimizers 
* Tuning the Activation Function (in what we call neuron activation)
* Tuning the Dropout Regularization Layer (dropout_rate, weight_constraint)
* Tuning Number of Neurons
* Tuning the Learning Rate and Momentum while using the SGD optimizer


Tuning hyperparameters of a neural network model can help improve the performance of the model. 
To tune these hyperparameters, we can use grid search from scikit-learn, which involves setting up a grid of possible values for the hyperparameters and retraining the model for each value of the parameter.A range of values are specified, and The combination which yields the highest accuracy will be selected as the best.

In the first example, a grid of hyperparameters (batch size and epochs) is defined, and a KerasClassifier model is created. Batch size refers to the number of samples that will be used to train the model in one iteration. The number of epochs refers to the number of times the entire training dataset will be passed through the model. GridSearchCV is used to exhaustively search the grid of hyperparameters to find the best combination of hyperparameters that maximizes the accuracy of the model. The best combination of hyperparameters is printed at the end.
In the second example, a grid of optimizers is defined, and a KerasClassifier model is created with a chosen batch size and epochs. Optimization algorithms help to reduce the loss function and improve the accuracy of the model. GridSearchCV is used to find the best optimizer that maximizes the accuracy of the model. The best optimizer is printed at the end. This process is repeated for the rest.



Results
The best hyperparameters and the highest accuracy achieved by the model are displayed in the console.
