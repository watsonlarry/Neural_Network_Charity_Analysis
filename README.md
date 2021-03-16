# Neural_Network_Charity_Analysis

## Overview

Working on behalf of the non-profit foundation AlphabetSoup we created binary classifier to predict whether grant applicants will be successful if funded. We processed th dataset provided by the foundation of 34,000+ organizations that have previously recieved funding and compiled, trained, and tested the neural network model. After the initial testing, we optimized the model for better results.

## Results

### Data Preprocessing

- Model's target variables: "IS_SUCCESSFUL" is the variable that measures funding success under the binary "1" and "0".

- Model's feature variables: variables "APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, SPECIAL_CONSIDERATIONS, INCOME_AMT, ASK_AMT" were featured to train the neural network.

- Model's removed variables: variables "EIN" and "NAME" had no potential for pattern training and were dropped.

### Compiling, Training, and Evaluating the Model

- Neurons, layers, and activation functions selected for neural network model: the initial testing was built w/ 120 nuerons across two hidden layers, with "relu"
& "sigmoid" activation functions. 

- Target model perfomance acheived: No. The Target accuracy is 75.0%. The initial trial was only able to achieve 72.6% accuracy and successive ooptimization attempts only resulted in 73-74% accuracy.

- Steps to increase model performance: During optimization trials I added neurons, hidden layers, and activation funtions. The final trial had 600 neurons and 7 hidden layers with "relu", "sigmoid", and "tanh" activation functions. Creading a more complex system seems to have positive effects on the accuracy, if not incredible transformative effects. A checkpoint system was implemented "ModelCheckpoint" from the tensorflow.keras library. The purposebing to save the model weights after it tests a set number of data points then, at any point, then reload the checkpoint weights and resume model training. After which we achieved marginally higher accuracy from the model.

## Summary

Disappointingly the target accuracy was not acheived through substantial manipulation of the nueural network's arrangement. In future tests I suggest a more thourough cleaning onf the dataset. It's possible that some superfluous elements still remain and are affecting the success rate of our model.







