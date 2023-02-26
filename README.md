# Module 20 Challenge: Neural Network Charity Analysis

## Overview of the analysis: 
   The purpose of this analysis is to use the features in the provided dataset, a CSV containing more than 34,000 organizations that have received funding from the client over the years, to create an optimized binary classifier using a neural network model that is capable of predicting whether future applicants will be successful if funded by our client, Alphabet Soup.
   

## Results: 
   Using bulleted lists and images to support your answers, address the following questions.

- Data Preprocessing
    - What variable(s) are considered the target(s) for your model?
The target for the model is the "IS_SUCCESSFUL" column variable.  It specifies the overall outcome of the funded organization as either successful or not.

    - What variable(s) are considered to be the features for your model?
The features for the model are the following column variables: 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'.  
    
    - What variable(s) are neither targets nor features, and should be removed from the input data?
The 'EIN' and 'NAME' column variables are neither targets nor features, and should be removed from the input data.  They offer no benefit to classifying the data.
    
    
- Compiling, Training, and Evaluating the Model
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?


    - Were you able to achieve the target model performance?
    - What steps did you take to try and increase model performance?

   There is a bulleted list that answers all six questions (15 pt)

## Summary: 
    Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
    
    There is a summary of the results (2 pt)
    There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)
