# Neural Network Model

# Overview of Project

From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organisations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organisation, such as:
- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organisation classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organisation type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special considerations for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

 # Methodology: Analytics Paradigm

- Preprocessing Data for a Neural Network Model
- Compile, Train, and Evaluate the Model
- Optimize the Model
- A Written Report on the Neural Network Model


# Define Strategy & Metrics
Resource: Python, numpy, pandas, sklearn, plotly.express, StandardScaler, OneHotEncoder, tensorflow.

# Analysis
![image](https://github.com/zquiroga/deep-learning-challenge/assets/118328051/55c0a2d1-4ba8-4777-b49f-6f5843870b93)

![image](https://github.com/zquiroga/deep-learning-challenge/assets/118328051/3460c4bb-552e-4046-a1fc-9cee4f547fb3)

This shows that it is only 73.17% accurate. 

# Data Preprocessing

- What variable(s) are the target(s) for your model?
  
  y = numerical_df["IS_SUCCESSFUL"].values  is the target for the model because this indicate that the applicant is successful.

- What variable(s) are the features for your model?
  
  IS_SUCCESSFUL is the feature column chosen data for the model.

- What variable(s) should be removed from the input data because they are neither targets nor features?
  
  EIN I removed from the input data because they are neither targets nor features.

# Compiling, Training, and Evaluating the Model

![image](https://github.com/zquiroga/deep-learning-challenge/assets/118328051/ec631249-a27a-477f-bcfc-cace4ea7157b)

- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  
  with three dense layers, and the total number of parameters is 37,981. The architecture includes layers with output shapes (80,), (30,), and (1,), respectively.
  

- Were you able to achieve the target model performance?
  
  The target for the model achieved a 79.07 % model performance despite optimization of the code

- What steps did you take in your attempts to increase model performance?

  in Application time - Determine which values to replace if counts are name_count <= 4 and Classification - Determine which values to replace if counts are less than < 1500.

# Optimize your model in order to achieve a target predictive accuracy higher than 75%

The biggest factor in achieving the target of more than 75% accuracy is by adding feature "NAME". By Adding this feature, the model was able to increase the accuracy to 79.15%. See results below.
by manipulating the "NAME" column and grouping less frequent values, you are performing feature engineering that seems to be benefiting the performance of your neural network model in terms of accuracy.

# Summary

the newly optimized model can predict, with 79.07% accuracy, whether an applicant will be successful in obtaining funding from Alphabet Soup. Occasionally, a feature that might
seem unimportant to a human turns out to be a significant factor. This suggests that the machine learning model carries inherent biases based on the choices made by its designer.

Using the same dataset, another more suitable model, such as Support Vector Machines (SVMs), would be less resource-intensive while still delivering good classification results.
Support Vector Machinesact like a judge, determining the best way to separate different groups of data, even in more complex scenarios. Additionally, SVMs are less computationally demanding, meaning they can achieve
good results without requiring excessive computational resources. 








  
  



  




  


  









  
