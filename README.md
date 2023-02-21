# Neural Network Charity Analysis


The purpose of this project is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. For this project, I implemented a Deep Learning model in order to evaluate more than 34,000 organizations that have received funding from Alphabet Soup over the years.


---


## Results


### Data Preprocessing

* What variable(s) are considered the target(s) for your model?

For this model, the target variable is determined with the "IS_SUCCESSFUL" column from the provided database. This column indicates whether or not the applicant was successful or not.

* What variable(s) are considered to be the features for your model?

For this model to provide an accuracy score above 75%, I considered the variables: NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.

* What variable(s) are neither targets nor features, and should be removed from the input data?

I removed the EIN varaible form the dataset since it didn't provided the model with the proper tools for accuracy.



### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?

For both the original and the optimized model, I used 2 hidden layers. There are 80 neurons in the first hidden layer and 30 in the second hidden layer. The idea for this amount of neurons in the model was to maximize the possible accuracy of the model. I also implemented the Relu activation for each of the hidden layers.

![Captura de pantalla 2023-02-20 a la(s) 18 47 42](https://user-images.githubusercontent.com/113866707/220220661-d2e95ed3-d67d-4493-beff-bfca038b048d.png)


* Were you able to achieve the target model performance?

On the first try, I was only able to reach an accuracy score of 72%, while in the optimization I reached 79% by using the NAME variable within the model.

### First try:
![Captura de pantalla 2023-02-20 a la(s) 18 49 13](https://user-images.githubusercontent.com/113866707/220220811-b27f9293-fb57-4732-b64b-c488ad78b7ef.png)

### Optimization:
![Captura de pantalla 2023-02-20 a la(s) 18 49 40](https://user-images.githubusercontent.com/113866707/220220883-659aefea-dd22-4ce6-b36f-bbe978a3c123.png)


* What steps did you take to try and increase model performance?
For the optimization model I decided to use the NAME variable within the model as an input variable. For NAME input variable, I had to bin components of the variable as "Other" in order to flatten the density components.


---


## Summary

* Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

The model achieve the desired accuracy score above 75% by employing and binning the NAME variable. With more time it could be possible to test the importance of other input variables and how much does the model improve.




