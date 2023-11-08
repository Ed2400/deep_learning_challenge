# deep_learning_challenge
Report of Neural Network Model

#Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

#Results

--Data Preprocessing--

1.- What variable(s) are the target(s) for your model?
  The IS_SUCCESFUL feature is the most important due to the type of model, which is a clasificatory.
2.- What variable(s) are the features for your model?
  After hotenconding the columns, all of them were able to be encluded in the model
3.-What variable(s) should be removed from the input data because they are neither targets nor features?
  The EIN and NAME are not used, because they are meatadata, which are not really necessary on classification.
  
--Compiling, Training, and Evaluating the Model--

1.-How many neurons, layers, and activation functions did you select for your neural network model, and why?
  The sigmoid activation was used in this model, I used three neurons and thre layers, this achieved a great accuracy, more      neurons or labels were unnecesary, considering that more neurons or labels were not affecting the accuracy of it.
2.- Were you able to achieve the target model performance?
  No, It performs around .73 accuracy, a decent value if we consider the amount of data. 
3.-What steps did you take in your attempts to increase model performance?
  By using the keras model, trying with different types of relu,tanh, and sigmoid active. Varying the amount of layers (6) and neurons(10).
  
--Summary--

The neural model demonstrated a decent precentage of accuracy of predicting the charity success, however the model can be improved by  using a PCA model to reduce the number of features correlated directly with the amount of noise. Preproccesing more, even increasing the volume of the data could help the amount of variance.
