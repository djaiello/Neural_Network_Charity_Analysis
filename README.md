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

       - Original Neural Network Model:
![image](https://user-images.githubusercontent.com/114360511/221687753-511ca52c-23e4-4bcb-924c-1a12747a98a4.png)

    - Were you able to achieve the target model performance?
    
 ![image](https://user-images.githubusercontent.com/114360511/221687803-0df0ba04-00c4-4c18-ae16-0669b6e9d0a9.png)
 
 
    - What steps did you take to try and increase model performance?
 
       - 1st Model Optimization Attempt:   
![image](https://user-images.githubusercontent.com/114360511/221686891-269b2a34-f9c4-4084-a781-f49d2fe8a540.png)
![image](https://user-images.githubusercontent.com/114360511/221687653-489e4541-1a2b-4987-9209-14edbd876612.png)

       - 2nd Model Optimization Attempt:   
![image](https://user-images.githubusercontent.com/114360511/221686977-7ee3a847-ad62-42c5-84ea-20eea4f11ab4.png)
![image](https://user-images.githubusercontent.com/114360511/221687120-1f84eaea-10f7-4d39-9ec7-b7ddd50b0e6c.png)

       - 3rd Model Optimization Attempt:   
![image](https://user-images.githubusercontent.com/114360511/221687406-88c29375-7f37-4c3e-98fc-cbf6ccdd3b49.png)
![image](https://user-images.githubusercontent.com/114360511/221687434-b17bf00d-a53e-427d-8365-9c59350e693a.png)


    

 
 

## Summary: 
    Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
    
    There is a summary of the results (2 pt)
    There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)
