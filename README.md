# Neural-Network-Charity-Analysis
# Module 20 Challenge: Neural Netowrk Charity Analysis - Deep Learning
## by Crystina Dang using Google Colaboratory, Jupyter Notebook within the mlenv Python environment


## Overview of the analysis:
The CSV, charity_data.csv, was provided by Alphabet Soup's business team containing more than 34,000 organzitions that have recieved funding over the years. Beks is seeking a machine learning model that can use this data set to predict future investments with 75% accuracy.


## Results: 
Inital test in AlphabetSoupCharity.ipynb:
![This is an image](https://github.com/crystdang/Neural-Network-Charity-Analysis/blob/main/Images/layers1.png)
![This is an image](https://github.com/crystdang/Neural-Network-Charity-Analysis/blob/main/Images/summary1.png)
![This is an image](https://github.com/crystdang/Neural-Network-Charity-Analysis/blob/main/Images/loss_acc1.png)

Intial test in AlphabetSoupCharity_Optimization.ipynb after additional bucketing and removal was done with the same model:
![This is an image](https://github.com/crystdang/Neural-Network-Charity-Analysis/blob/main/Images/layers2.png)
![This is an image](https://github.com/crystdang/Neural-Network-Charity-Analysis/blob/main/Images/loss_acc2.png)



### Data Preprocessing
What variable(s) are considered the target(s) for your model?
- The target is the "IS_SUCCESSFUL" column that contains 1 for yes and 0 for no.

What variable(s) are considered to be the features for your model?
- The features are the "APPLICATION_TYPE" "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "INCOME_AMT", and "ASK_AMT" columns.

What variable(s) are neither targets nor features, and should be removed from the input data?
- Removed variables are the "EIN", "NAME", "STATUS", and "SPECIAL_CONSIDERATIONS" columns.



### Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?
- 

Were you able to achieve the target model performance?
- No

What steps did you take to try and increase model performance?
- Removing additional unnecessary columns, ID, status and special considerations
- bucket asking amount

- additional layer, did not help
- Adjusting the activation to tanh
- adjusting neurons to be 2-3 times the amount of inputs


 
### Summary: 
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

The sigmoid function values are normalized to a probability between 0 and 1, which is ideal for binary classification.
The tanh function can be used for classification or regression, and it expands the range between -1 and 1.
The ReLU function is ideal for looking at positive nonlinear input data for classification or regression.
The Leaky ReLU function is a good alternative for nonlinear input data with many negative inputs.

A best model hyperparameters test was run for 4 hours and 507 tests were run to reach the best accuracy of 73%:
![This is an image](https://github.com/crystdang/Neural-Network-Charity-Analysis/blob/main/Images/hyperparameters_test.png)
![This is an image](https://github.com/crystdang/Neural-Network-Charity-Analysis/blob/main/Images/best_model.png)