# Neural_Network_Charity_Analysis
## Overview: 
The purpose of this analysis was to practice using neural networks and deep learning models. During the process, we learned how to:
- Compare the differences between traditional machine learning classification, regression models and the neural network models.
- Describe the perceptron model and its components.
- Implement neural network models using TensorFlow.
- Explain how different neural network structures change algorithm performance.
- Preprocess and construct datasets for neural network models.
- Compare the differences between neural network models and deep neural networks.
- Implement deep neural network models using TensorFlow.
- Save trained TensorFlow models for later use.
## Results: 
- Data Preprocessing
  - "IS_SUCCESSFUL", which indicates if a charity used their donations effeectively, was the target for the model.
  - "APPLICATION_TYPE" and "CLASSIFICATION" were the features for the model.
  - "EIN" and "NAME", which were identificatoins models, were not targets nor features. Therefore, they were removed from the input data.
- Compiling, Training, and Evaluating the Model
  - There were 2 hidden layers.
  - The first hidden layer contained 80 neurons.
  - The second hidden layer contained 25 neurons.
  - The hidden layers used relu activation.
  - the output layer used sigmoid activation.
  - I was not able to achieve target model performance.
  - In an effort to increase performance, I performed the following tasks:
    - changed the number of neurons in hidden layers
     <img width="637" alt="attempt1" src="https://user-images.githubusercontent.com/94420548/167507749-866532cf-0757-46bd-99d2-726ffd7507f1.png">
     
      This achieved a loss of 0.6911 and an accuracy: 0.5324.
      
    - add a 3rd hidden layer
     <img width="630" alt="attempt2" src="https://user-images.githubusercontent.com/94420548/167507772-53778f5a-cf5a-4e74-9e74-dab52109e7ec.png">
     
      This achieved a loss of 0.6911 and an accuracy: 0.5324.
      
    - changed the activation function
    <img width="630" alt="attempt3" src="https://user-images.githubusercontent.com/94420548/167507782-454ec5f1-7296-46d0-a52b-7906010843ac.png">
    
     This achieved a loss of 8.2126 - accuracy: 0.4676.
     
 None of the models achieved target performance.

## Summary: 
Every model needs significant work. We need an alternative model. We could look at other variables, such as ASK_AMT. It may be possible to bin ranges in order to decrease unique values, which may improve the accuracy of the models.
