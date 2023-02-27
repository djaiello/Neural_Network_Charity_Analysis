# Module 20 Challenge: Neural Network Charity Analysis

## Overview of the analysis: 
   The purpose of this analysis is to use the features in the provided dataset, a CSV containing more than 34,000 organizations that have received funding from the client over the years, to create an optimized binary classifier using a neural network model that is capable of predicting whether future applicants will be successful if funded by our client, Alphabet Soup.
   

## Results:
- Data Preprocessing
    - What variable(s) are considered the target(s) for your model?
The target for the model is the "IS_SUCCESSFUL" column variable.  It specifies the overall outcome of the funded organization as either successful or not.

    - What variable(s) are considered to be the features for your model?
The features for the model are the following column variables: 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'.  
    
    - What variable(s) are neither targets nor features, and should be removed from the input data?
The 'EIN' and 'NAME' column variables are neither targets nor features, and should be removed from the input data.  They offer no benefit to classifying the data.
    
    
- Compiling, Training, and Evaluating the Model
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?
I selected to use a basic neural network to start(as seen below), with one hidden layer containing 80 neurons and using the RELU activation function.  I chose to begin with a basic model to limit processing power and get a benchmark for how well a simple netwrok would perform on a fairly straightforward tabular dataset.  I chose the RELU activation function because it is considered the standard default for nonlinear data and I chose 80 neurons following the general rule of using ~2-3 times the number of input features columns, which was 44 in this case. 
        - Original Neural Network Model:
![image](https://user-images.githubusercontent.com/114360511/221687753-511ca52c-23e4-4bcb-924c-1a12747a98a4.png)

    - Were you able to achieve the target model performance?
A shown in the following image, the basic model only achieved an accuracy of ~73%.  The target model performance for this project is 75%, therefore it came up just short.
![image](https://user-images.githubusercontent.com/114360511/221687803-0df0ba04-00c4-4c18-ae16-0669b6e9d0a9.png)
 
    - What steps did you take to try and increase model performance?
    
Trying to increase the model performance to reach the established goal of 75%, three attempts were made to optimize the model and achieve the goal:

        - 1st Model Optimization Attempt Changes(from the original): 
            - Noisy variable, 'SPECIAL_CONSIDERATIONS' was removed from features.
            - Additional 2nd hidden layer was added
            - Additional 40 neurons are added to hidden layers
            
![image](https://user-images.githubusercontent.com/114360511/221686891-269b2a34-f9c4-4084-a781-f49d2fe8a540.png)
![image](https://user-images.githubusercontent.com/114360511/221687653-489e4541-1a2b-4987-9209-14edbd876612.png)

        - 2nd Model Optimization Attempt Changes(from the original):
            - Noisy variable, 'SPECIAL_CONSIDERATIONS' was removed from features.
            - Additional 2nd hidden layer was added
            - Additional 40 neurons are added to hidden layers
            - The activation function of the 2nd hidden layer was changed, to "tanh" for optimization
            
![image](https://user-images.githubusercontent.com/114360511/221697763-824829c3-14b6-46e1-b2b3-cfb197fcc85f.png)
![image](https://user-images.githubusercontent.com/114360511/221687120-1f84eaea-10f7-4d39-9ec7-b7ddd50b0e6c.png)

        - 3rd Model Optimization Attempt Changes(from the original):
            - Noisy variable, 'SPECIAL_CONSIDERATIONS' was removed from features.
            - Additional 2nd hidden layer was added
            - Reduced the 1st hidden Layer to 20 noded from 40
            - Added 8 nodes to the 2nd hidden layer
            - The activation function of the Output layer was changed, to "softmax" for optimization
            - Increase the epochs to 150
            
![image](https://user-images.githubusercontent.com/114360511/221687406-88c29375-7f37-4c3e-98fc-cbf6ccdd3b49.png)
![image](https://user-images.githubusercontent.com/114360511/221687434-b17bf00d-a53e-427d-8365-9c59350e693a.png)


## Summary: 
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
    
    There is a summary of the results (2 pt)
    There is a recommendation on using a different model to solve the classification problem, and justification (3 pt)
