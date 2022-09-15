# Neural_Network_Charity_Analysis

## Overview of Analysis
The purpose of this analysis is to predict whether applicants will be successful if funded by Alphabet Soup using a binary classifier. Data will be taken from a CSV containing organizations that have received funding from Alphabet Soup over the years, and that data will be analyzed to create a prediction.

## Results 

### Data Preprocessing
- The variable that is considered the target for the model is the "IS_SUCCESSFUL" variable.
- The variables that are considered the features for the model would be all the other variables except the "IS_SUCCESSFUL" variable.
- The variables that were neither targets nor features, and that were removed from the input data are "EIN" and "NAME".

### Compiling, Training, and Evaluating the Model
- In the neural network model, there were 2 layers, with the first layer containing 80 neurons and the second containing 30. This was because there were 41 features, and as a rule of thumb, the first layer's neurons should be about double of the number of features, hence the 80 neurons in the first layer. The second layer contained 30 neurons as it is about half of the first layer. Lastly, the activation functions that was used for the first and second layer is the ReLu function and for the outer layer was the Sigmoid function.

![original](https://user-images.githubusercontent.com/64383146/190311360-236d1c07-d7fb-4b03-a86d-fb0d86f7654e.png)

- The image above shows the target model performance at an accuracy of 73%, so I was not able to achieve the target model performance of 75%.

![first_attempt](https://user-images.githubusercontent.com/64383146/190313772-790bd418-a44b-403b-9760-f0114fb12009.png)

- The first step I took to try and increase the model performance was to increase the number of neurons in the layers, changing the first layer from 80 to 120 neurons and the second layer from 30 to 80 neurons. The image above shows that the accuracy was 72.85%, meaning that this model was not optimized.

![second_attempt](https://user-images.githubusercontent.com/64383146/190314691-a86a0015-cc69-41c2-866c-cbd037daa964.png)

- The second step I took to try and increase the model performance was to increase the number of layers in the model. The image above shows that the accuracy was 72.93%, a bit better than the first step but it was still not optimized.

![third_attempt](https://user-images.githubusercontent.com/64383146/190315625-cfbe3489-6126-4483-9cbf-f5f52c4f3743.png)


- The last step I tried was to change the activation functions for the layers. I changed activation functions for both the layers from the ReLu function to the Sigmoid function. The image above shows that the accuracy was 73.01%, meaning that the optimization was the same as the original model.

## Summary
The overall results of the deep learning model were that the accuracy was not able to reach the optimized amount of 75%. Though it was able to get close, it was not able to reach it even after changing some features.

A different model that can be used to solve this classification problem could be the Random Forest classifier as it is known to have a high accuracy rate and high interpretability.

