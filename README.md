** Neural_Network_Charity_Analysis **

 # *Overview of the analysis* 

The purpose of the project is to predict whether applicants will   be successful if funded by Alphabet Soup.
  By using the knowledge of machine learning and neural networks, used the features in the provided dataset. 


*Data Preprocessing*

The variables that are considered to be the features for your model

   EIN and NAME—Identification columns
   APPLICATION_TYPE—Alphabet Soup application type
   AFFILIATION—Affiliated sector of industry
   CLASSIFICATION—Government organization classification
   USE_CASE—Use case for funding
   ORGANIZATION—Organization type
   STATUS—Active status
   INCOME_AMT—Income classification
   SPECIAL_CONSIDERATIONS—Special consideration for application
   ASK_AMT—Funding amount requested
   IS_SUCCESSFUL—Was the money used effectively


The variable(s) that are neither targets nor features,  removed from the input data
  *EIN
  *NAME


*Compiling, Training, and Evaluating the Model*

  * For the initial attempt at model, two layers, with 80 and 30 neurons respectively (both "relu" type) were used. The activation feature of "sigmoid" was used. This was presented by the client as the starting point for model creation, allowing the analyst two further adjust in order to increase optimization.


 * The model performance was set at 75%. Unfortunately, the current model only achieved an accuracy rating of 74.09% on epochs 96 and 99. An overall accuracy average of 72.98% was achieved.
 
 ** Attempts done three times and following are the end points **
 
Attempt:1

 Hidden layer one: tanh type - 80 neurons
 Hidden layer two: relu type - 30 neurons
 Activation: sigmoid
 Highest accuracy/epoch: 74.08%, epoch 81 of 100
 Overall accuracy average: 72.79%
 
Attempt 2:

 Dropped noisy data of ASK_AMT
 Hidden layer one: tanh type - 80 neurons
 Hidden layer two: relu type - 50 neurons
 Hidden layer three: sigmoid type - 30 neurons
 Activation: relu
 Highest accuracy/epoch: 74.00%, epoch 89 of 100
 Overall accuracy average: 73.04%
 
Attempt 3:

 Dropped noisy data of ASK_AMT
 Hidden layer one: sigmoid type - 100 neurons
 Hidden layer two: sigmoid type - 75 neurons
 Hidden layer three: relu type - 50 neurons
 Hidden layer four: relu type - 25 neurons
 Activation: sigmoid
 Highest accuracy/epoch: 74.09%, epoch 99 of 100
 Overall accuracy average: 72.92%

** Final thought **

 The initial setup for the model did not perform at the required level, coming in at 72.98%. 
 Through iterative design, the model was adjusted and obtained an increased rating of 73.04% on the second optimization attempt.
 All other models had lower final accuracies than the initial model. 
 For this, it can be seen that changing the number of hidden layers and neurons had a negligible effect on increasing model accuracy.







