# deep-learning-challenge
Module 21 Challenge deep-learning-challenge
***
# Introduction

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

# Findings
## Data Processing
### What variable(s) are the target(s) for your model?
* The 'IS_SUCCESSFUL' column from application_df is the target variable, this is what we are trying to predict. This shows if the money was used effectively.
### What variable(s) are the features for your model?
* The feature variables we used are:
    * AFFILIATION—Affiliated sector of industry
    * CLASSIFICATION—Government organization classification
    * USE_CASE—Use case for funding
    * ORGANIZATION—Organization type
    * STATUS—Active status
    * INCOME_AMT—Income classification
    * SPECIAL_CONSIDERATIONS—Special considerations for application
    * ASK_AMT—Funding amount requested
### What variable(s) should be removed from the input data because they are neither targets nor features?
* Identification columns: The "EIN" and "NAME" columns are identification columns that typically provide unique identifiers for each organization. These columns usually have no direct impact on the target variable and can be dropped without affecting the model's accuracy.
    * Note: for the Optimized version, only "EIN" is removed so we can use "NAME" as a part of the features

## Compiling, Training, and Evaluating the Model
### How many neurons, layers, and activation functions did you select for your neural network model, and why?
* The 1st/original neural network model, I used a three-layer architecture with a specific choice for the number of neurons, layers, and activation functions.
    * input_features = len(X_train_scaled[0])
    * hidden_nodes_layer1 =  100
    * hidden_nodes_layer2 = 60
    * output_nodes_layer3 = 1

![model]("Resources/Original_model.png")
