# Neural_Network_Charity_Analysis

## Overview of Analysis

This analysis will focus on creating a deep learning neural network model to predict which foundations are worth donating to and which are too high risk. In this analysis, we will test and optimize our models to determine which charities to invest in.

## Results

### Data Preprocessing

  1. What variable(s) are considered the target(s) for your model?
      The variable that is considered the target for the model is the "IS_SUCCESSFUL" column.
  
  2. What variable(s) are considered to be the features for your model?
      Every column minus the "IS_SUCCESSFUL" column is a feature in the model.
  
  3. What variable(s) are neither targets nor features, and should be removed from the input data?
      The varibales that are neither a target or feature is the "EIN" and "Name" columns which are dropped. They do not provide any signficiant value to the model.
  
### Compiling, Training, and Evaluating the Model

  1. How many neurons, layers, and activation functions did you select for your neural network model, and why?
      In the optimized model, layer 1 started with 110 neurons with a relu activation. For layer 2, it dropped to 80 neurons and continued with the relu activation.
      From there, the sigmoid activation seemed to be the better fit for layers 3 (40 neurons) and layer 4 (20 neurons).
      
  2. Were you able to achieve the target model performance?
      The model was not able to reach the target 75%. 
      
  3. What steps did you take to try and increase model performance?
      Columns were reviewed and the STATUS and SPECIAL_CONSIDERATIONS columns were dropped as well as increasing the number of neurons and layers. 
      
  ## Summary

The relu and sigmoid activations yielded a 72.5% accuracy, which is the best the model could produce using various number of neurons and layers. The next step should be to try the random forest classifier as it is less influenced by outliers.

