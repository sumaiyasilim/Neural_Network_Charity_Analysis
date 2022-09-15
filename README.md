# Neural_Network_Charity_Analysis

## Overview of Analysis
The purpose of this analysis is to predict whether applicants will be successful if funded by Alphabet Soup using a binary classifier. Data will be taken from a CSV containing organizations that have received funding from Alphabet Soup over the years, and that data will be analyed to create a predicition.

## Results 

### Data Preprocessing
- The variable that is considered the target for the model is the "IS_SUCCESSFUL" variable
- The variables that are considered the features for the model would be all the other variables except the "IS_SUCCESSFUL" variable
- What variables are neither targets nor features, and should that were removed from the input data are "EIN" and "NAME"

### Compiling, Training, and Evaluating the Model
- In the neural network model, there were 2 layers, with the first layer containing 80 neurons and the second containing 30. This was because there were 41 features, and as a rule of thumb, the first layer's neurons should be about double of the amount of features, hence the 80 neurons in the first layer. The second layer contained 30 neurons as it is about half of the first layer. Lastly, the activation functions that was used  
