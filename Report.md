# Alphabet Soup Deep Learning Model Performance Report

## Overview of the Analysis

The purpose of this analysis was to develop a deep learning model using TensorFlow and Keras to predict the success of funding applicants for Alphabet Soup based on various input features.

## Results

### Data Preprocessing

**Target Variable**: The target variable for the model is IS_SUCCESSFUL, which indicates whether the funding application was successful.

**Features**: The features for the model include APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, and SPECIAL_CONSIDERATIONS.

**Removed Variables**: Variables EIN and NAME were removed from the input data as they were neither targets nor features.

### Compiling, Training, and Evaluating the Model

**Neurons, Layers, and Activation Functions**:
For the first model (AlphabetSoupCharity.ipynb), two hidden layers with 80 and 30 neurons were selected, respectively, using the ReLU activation function.
For the second model (AlphabetSoupCharity_Optimization.ipynb), the complexity was increased with four hidden layers having 100, 50, 20, and 10 neurons, respectively, using the ReLU activation function. The output layer for both models used the sigmoid activation function.

**Model Performance**:
The first model achieved an accuracy of 72.7%.
The second model achieved an accuracy of 72.4%.

**Target Model Performance**: While the target model performance of over 75% accuracy was not achieved for either model, with the first model achieving an accuracy of 72.7% and the second model achieving 72.4%, they provide a good starting point for further optimization.

**Steps Taken** :

Adjusting Binning:
Increased the cutoff value for binning rare occurrences in columns from 500 to 1000 in the second model, which did not significantly improve model accuracy.
Dropping Columns:
Explored dropping more or fewer columns from the input data, but the model's accuracy remained lower or similar.
Other Attempts:
Increased the number of hidden layers and neurons in the second model.
Used different activation functions for the hidden layers.
Increased the number of epochs to 120 and 170 in the second model.

**Steps to Increase Performance**:
Increased complexity with additional hidden layers and neurons in the second model.
Adjusted binning for rare occurrences in columns.
Increased the number of epochs to 200 in the second model.

## Summary

The deep learning models developed for Alphabet Soup aimed to predict the success of funding applicants based on various input features. The first model (AlphabetSoupCharity.ipynb) used two hidden layers with 80 and 30 neurons, achieving an accuracy of 72.7%. The second model (AlphabetSoupCharity_Optimization.ipynb) increased complexity with four hidden layers having 100, 50, 20, and 10 neurons, but achieved a slightly lower accuracy of 72.4%.

Despite not achieving the target model performance of over 75% accuracy, both models provided valuable insights. Adjustments were made in the second model, including increasing the cutoff value for binning rare occurrences, exploring different neural network architectures, and increasing the number of epochs to 200. These attempts aimed to improve model accuracy but did not yield significant improvements.

Moving forward, further optimization could involve fine-tuning hyperparameters, exploring more complex neural network architectures, and applying regularization techniques. Overall, while the models showed moderate success, there is room for improvement to enhance their predictive performance for funding application outcomes.
