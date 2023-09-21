# CountVectorizer.ipynb README

# Table of Contents
1. Overview
2. What is Randomized Search CV
3. How do we implement RandomizedSearchcV as a funtion

# Overview
This document presents the definitions for Randomized Search CV. The implementation is done through two tasks which are self explanatory. 


# What is Randomized Search CV?
Randomized Search CV, or Randomized Search Cross-Validation, is a widely used Hyperparameter Tuning technique. A fixed number of parameters are sampled randomly based on the settings, with sampling performed with replacement if at least one parameter is provided, and without replacement if all parameters are presented in the predefined search space. Using these parameters, the models performace is evaluated using cross validation for each combination of data. The combination of data is defined by user through the number of folds and thus, the values are aggregated and then the best hyperparameters are selected. 

Randomized Search CV has been found to be powerful due to its reduced processing time."

# How do we implement RandomizedSearchCV as a function
1. Generate 10 unique values(uniform random distribution) in the given range "param_range" and store them as "params". 
Example: if param_range = (1, 50), we need to generate 10 random numbers in range 1 to 50
2. Divide numbers ranging from  0 to length of X into groups= folds
Example: folds=3, and len(x_train)=100, we can divide numbers from 0 to 100 into 3 groups group 1: 0-33, group 2:34-66, group 3: 67-100
3. For each hyperparameter generated in step 1:
Using the above groups we have created in step 2 the cross-validation is done as follows
<br> Example:
    1. All groups except group 3, i.e. 0-66 are considered as train data and last group (group 3) i.e. 67-100 as test data, and find train and test accuracies
    2. Keep group 1+group 3 i.e. 0-33, 67-100 as train data and group 2: 34-66 as test data, we find train and test accuracies
    3. Keeping group 2+group 3 i.e. 34-100 as train data and group 1: 0-33 as test data, we find train and test accuracies
    4. Based on the 'folds' value the same procedure is repeated
    5. The mean of train accuracies of above 3 steps is calculated and stored in a list "train_scores"
    6. The mean of test accuracies of above 3 steps is calculated and stored in a list "test_scores"
    7. The "train_scores" and "test_scores" are returned
<\br>