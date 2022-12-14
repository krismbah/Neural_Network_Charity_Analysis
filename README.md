# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to use the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. In order to predict whether applicants will be successful if funded by Alphabet Soup, the following tasks are to be completed: 

1. Preprocessing Data for a Neural Network Model.
2. Compile, Train, and Evaluate the Model.
3. Optimize the Model.


## Results


***Deliverable 1: Preprocessing Data for a Neural Network Model***
Using knowledge of Pandas and the Scikit-Learn’s StandardScaler(), preprocess the dataset in order to compile, train, and evaluate the neural network model later in Deliverable 2:

Figure 1:

![Image1](https://raw.githubusercontent.com/krismbah/Neural_Network_Charity_Analysis/main/D1.png)



***Deliverable 2: Compile, Train, and Evaluate the Model***
Using knowledge of TensorFlow, design a neural network, or deep learning model, to create a binary classification model that can predict if an Alphabet Soup–funded organization will be successful based on the features in the dataset. Think about how many inputs there are before determining the number of neurons and layers in the model. Once completing that step, compile, train, and evaluate the binary classification model to calculate the model’s loss and accuracy:

Figure 2:

![Image2](https://raw.githubusercontent.com/krismbah/Neural_Network_Charity_Analysis/main/D2.png)



***Deliverable 3: Optimize the Model***
Using knowledge of TensorFlow, optimize the model in order to achieve a target predictive accuracy higher than 75%:

Figure 3:

![Image3](https://raw.githubusercontent.com/krismbah/Neural_Network_Charity_Analysis/main/D3.png)


Figure 3.1:

![Image3.1](https://raw.githubusercontent.com/krismbah/Neural_Network_Charity_Analysis/main/D3.1.png)



### Data Preprocessing 
* "What variable(s) are considered the target(s) for your model?" The 'IS_SUCCESSFUL' column is considered to be the target of this model due to being a binary flag indicating the applicant will be successful if funded by Alphabet Soup.


* "What variable(s) are considered to be the features for your model?" The following variables are considered the features for this model; 'EIN', 'NAME', 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', and 'ASK_AMT'.



* "What variable(s) are neither targets nor features, and should be removed from the input data?" 'EIN' was removed due to being an ID number rather than a metric which could confuse the model into thinking it was significant.


### Compiling, Training, and Evaluating the Model
* "How many neurons, layers, and activation functions did you select for your neural network model, and why?" 100 neurons in the first layer, 30 neurons in the second layer, and 1 neuron in the third layer. The Sigmoid activation function was selected for each layer due to better accuracy.


* "Were you able to achieve the target model performance?" Yes, accuracy was 78.05 percent.


* "What steps did you take to try and increase model performance?" Adding a third layer with a sigmoid activation function in the first layer with 100 neurons.



## Summary


In Summary, the model accuracy was successfully optimized above the 75 percent threshold and reached a predictive accuracy level of 78 percent. The following models were considered using the same parameters; Logistic Regression, Random Forest, and Support Vector Machine. Both the Logistic Regression and Random Forest models resulted in predictive accuracy levels below the current optimized model. The Support Vector Machine model did not produce a result. My recommendation would be to use the current optimized model. However, using other parameters and models may produce better results if experimented.
