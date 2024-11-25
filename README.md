# Challeng 19  (neural-network-challenge-2)

This challenge asks to create a neural netork to perform 2 functions:
1. Determine if an employee is an attrition risk
2. Determine if an employee is better suited to a different department from an HR perspective.

This will be done as part of the same branched neural network model. 


## Scaling and cleaning the data
The targets of the provided data are the following columns
1. Department
2. Attrition

The remaining data will have 10 attributes selected against which the data model is to be run.  

All data is first scaled throught the ```StandardScaler```.   The target data is transformed utilizing ```OneHotEncoder```.  


## Creating the model

The model data is processed through a branched neural network.  THere are 2 shared layers to process and the the model is then branched to predict the outcomes for the department and attrition targets. 

The model is compiled with the Adam optimizer and summarized to verify the structure of the model.  

Once ready, model is trained with the preprocessed data and an evaluation is performed on the test data set.  

Accuracy is displayed for both targets. 