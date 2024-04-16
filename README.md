## Overview
The purpose of this analysis is to develop a predictive model using deep learning techniques to determine the success of organizations funded by Alphabet Soup. By preprocessing the provided dataset and creating a binary classification model, we aim to predict whether an organization will utilize the funding effectively.

### Data Preprocessing:

- **Target Variable(s):**
  - `IS_SUCCESSFUL`: Indicates whether the funding provided to an organization was used effectively.

- **Feature Variable(s):**
  - `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, `ASK_AMT`.

### Compiling, Training, and Evaluating the Model:

- **Neurons, Layers, and Activation Functions:**
  - **Input Layer:** 26 neurons corresponding to the number of input features.
  - **Hidden Layers:** Two hidden layers with 21 neurons each, utilizing the hyperbolic tangent (tanh) activation function.
  - **Output Layer:** Single neuron with a sigmoid activation function for binary classification.

- **Achievement of Target Model Performance:**
  - The model achieved a loss of 0.5588 and an accuracy of 72.67% on the test data.

- **Steps Taken to Develop Model:**
  - Used multiple hidden layers for higher accuracy.
  - Utilized the tanh activation function for handling non-linearities.
  - Set epochs = 100.

## Summary
For model creation, a neural network architecture was designed with an input layer of 26 neurons (matching the number of features) followed by two hidden layers with 21 neurons each, using the tanh activation function. The output layer consisted of a single neuron with a sigmoid activation function for binary classification.

After compiling, training, and evaluating the model, it achieved a loss of 0.5588 and an accuracy of 72.67% on the test data.

The deep learning model successfully predicts the effectiveness of funding for Alphabet Soup-funded organizations with an accuracy exceeding the target threshold. Despite achieving a reasonably high accuracy, there is room for further optimization to improve model performance. Experimentation with additional hidden layers, nodes, using `keras_tuner`, and alternative activation functions could be explored in future iterations to enhance predictive accuracy.

