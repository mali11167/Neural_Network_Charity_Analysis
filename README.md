# Neural_Network_Charity_Analysis
## Overview
In this project we will be performing machine learning and neural networks. We use the features in the provided dataset to create a binary classifier that is 
able to predict whether applicants will be successful if funded by Alphabet Soup. The idea is to see different architecture of the neural network to get better results.
## Results
We used Pandas and the Scikit-Learn’s StandardScaler(), we need to preprocess the dataset in order to compile, train, and evaluate the neural 
network model. We analyzed as follows:
* We took application type as our target variable and then classifying it and merging it with original data with the asking amount information. 
* The variable that were the features was "Is Successful".
* The varibales that were not needed were name and ein and those were removed. 

In the first part we dropped the name and ein columns as they were unnecessary to predict if the applicant is successful if funded by Alphabet soup. 
Next we looked at any unique values and found:

![unique](https://user-images.githubusercontent.com/91965321/158000739-e4dc26c9-8230-4eea-ae4c-9864f8a0208a.jpg)

We did the visualization through density plot for application and calssification:

![image](https://user-images.githubusercontent.com/91965321/158000766-1cb026f5-e77b-4b51-8c46-3bca2d3cd21f.png)

We did the training and testing of the dataframe and ran a deep neural network with two hidden layers, 8,5 neurons, and no of epochs to be 5. With running this
model we got the accuracy level of 57%. This shows that this model is not that accurate as the level of accuracy is low.
![accuracy](https://user-images.githubusercontent.com/91965321/158000875-ca188eb8-6e5b-4615-b77f-b73a9eb1393d.jpg)

 For the second iteration, this is an updated example of the NN architecture using the same dataset. We added three hidden layers and numberof neurons were 100,
 30, 10 essentially. This made a huge difference in the accuracy of the architecture as it was 72% with 100 epochs. We later saved the results to hdf5 file.
 ![acc ](https://user-images.githubusercontent.com/91965321/158001040-98206c26-ad81-451b-9fc6-21f2342eed86.jpg)

## Summary
According to our analysis the number of hidden layers and number of neurons made a huge difference in the accuracy of a the model. The more the hidden layers 
and more neurons eventually increased the accuracy of the model. But to the downside of this was that the accuracy of this model could not go more then 72% as
more hidden layers and more neurons and more epochs took a long time to run and decreased the accuracy. So I think for the model we ran and the setup that was
done this is the best that could come out of this.
