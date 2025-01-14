## Overview of the Analysis

The purpose of this analysis is to develop a neural network model to predict the success of charity donations based on various features of the charity applications. The goal is to identify which factors contribute to successful fundraising efforts and use this information to optimize future donation strategies.
## Results
* Data Preprocessing

    Target Variable:

        IS_SUCCESSFUL: This variable indicates whether a donation application was successful (1) or not (0).

    Feature Variables:

        All other variables in the dataset after dropping the non-beneficial ID columns EIN and NAME.

        This includes variables such as APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

    Variables Removed:

        EIN and NAME: These columns are neither targets nor features and do not contribute to the prediction.

* Compiling, Training, and Evaluating the Model

    * Model Structure:

        First Try:

            Neurons: 8 in each hidden layer

            Layers: 2 hidden layers

            Activation Functions: ReLU for hidden layers, Sigmoid for output layer

            Reason: A simple model to start with and evaluate baseline performance

       Second Try:

            Neurons: 16 in each hidden layer

            Layers: 2 hidden layers

            Activation Functions: ReLU for hidden layers, Sigmoid for output layer

            Reason: Increased number of neurons to potentially capture more complex patterns

        Third Try:

            Neurons: 24 in each hidden layer

            Layers: 2 hidden layers

            Activation Functions: Tanh for hidden layers, Sigmoid for output layer

            Reason: Changed activation function to Tanh and increased neurons to further explore performance improvements

    * Target Model Performance:

        The target model performance was not achieved as the accuracy remained around 72-73% across different attempts.

    * Steps to Increase Model Performance:

        Tried different combinations of neurons and activation functions in hidden layers.

        Increased the number of epochs to allow more training iterations.

## Summary

The overall results of the deep learning model indicate that the accuracy of the model is around 72-73%, which suggests that the model has room for improvement. The changes in the model structure, including increasing neurons and changing activation functions, did not significantly enhance the performance.