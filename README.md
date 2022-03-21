# Neural_Network_Charity_Analysis
## Overview of the analysis
This project is designed to help Beks to work to help the Alphabet Soup foundation predict where to make investments. Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. This project used the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.
## Results
### Data Preprocessing
 - What variable(s) are considered the target(s) for your model?  
 The "IS_SUCCESSFUL" variable is considered the target for my model.  
 
 - What variable(s) are considered to be the features for your model?  
 The "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", "ASK_AMT" are the features for our model.  
 
 - What variable(s) are neither targets nor features, and should be removed from the input data?  
 The "EIN" and "NAME" columns are neither targets nor features and should be removed from the input data.
 
### Compiling, Training, and Evaluating the Model
 - How many neurons, layers, and activation functions did you select for your neural network model, and why?  
 This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons respectively with a ReLU function.  
 ![D2](https://github.com/JosephineYang228/Neural_Network_Charity_Analysis/blob/e5ce1a8cc14d1e6116a02e01e1c00de235ec4eb2/Resources/images/D2.png)  
 
 The reason I choose this function is that ReLU function returns a value from 0 to infinity, so any negative input through the activation function is 0. It is the most used activation function in neural networks due to its simplifying output.  
 ![DL%20&%20RF](https://github.com/JosephineYang228/Neural_Network_Charity_Analysis/blob/e5ce1a8cc14d1e6116a02e01e1c00de235ec4eb2/Resources/images/DL%20&%20RF.png)
 
 - Were you able to achieve the target model performance?  
 Since the accuracy is 62% in Deverliable 1 & 2, and is 73% after I optimize my model, which is still lower than 75%, I CANNOT say it achieve the target model performance.  
 ![D2%20Eval](https://github.com/JosephineYang228/Neural_Network_Charity_Analysis/blob/e5ce1a8cc14d1e6116a02e01e1c00de235ec4eb2/Resources/images/D2%20Eval.png)  
 ![D3%20Eval](https://github.com/JosephineYang228/Neural_Network_Charity_Analysis/blob/e5ce1a8cc14d1e6116a02e01e1c00de235ec4eb2/Resources/images/D3%20Eval.png)
 
 - What steps did you take to try and increase model performance?  
 I tried to increase the model performance by creating more bins for rare occurances in columns, increasing the number of values in some bins, adding more neurons to the hidden layers and increasing the number of epochs.
 
## Summary
The loss of my optimized model is 0.60, and the optimized accuracy is 73%.  
![D3%20Eval](https://github.com/JosephineYang228/Neural_Network_Charity_Analysis/blob/e5ce1a8cc14d1e6116a02e01e1c00de235ec4eb2/Resources/images/D3%20Eval.png)  

### Recommendation
Maybe I could try some more methods to improve the model accuracy by drop off useless coloums or using a differnet activation function.
