Alphabet Soup Charity Deep Learning Challenge

Overview:
The purpose of this analysis is to create a classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

Results:

Data Preprocessing

What variable(s) are the target(s) for your model?
-The variable that was targeted in my initial model was the 'is_succesful' column

![Alt text](Starter_Code/Code_Snippet/targets.png)

What variable(s) are the features for your model?
-The features were the every other column in the application_df except for 'EIN' and 'Name' (Name was added in the optimization models)

What variable(s) should be removed from the input data because they are neither targets nor features?
-As mentioned, the variables that were removed from the initial model because they were neither targets or features were the 'EIN' and 'Name'

![Alt text](Starter_Code/Code_Snippet/features.png)


Compiling, Training & Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
-I used 80 and 30 neurons, 3 layers and 2 activation functions in my initial neural network model and first optimization attempt. Then I changed the neurons to 100, 30 and 10  and added another layer in my second optimization attempt. I added more layers in the optimization to increase the model's capacity.

![Alt text](Starter_Code/Code_Snippet/initial_neural_network.png)
![Alt text](Starter_Code/Code_Snippet/final_neural_network.png)

Were you able to achieve the target model performance?
-Yes, I was able to achieve the target model performance on the third iteration of my model

What steps did you take in your attempts to increase model performance?
-In my first attempt to increase model performance I changed up the binning but it actually made the model less accurate. In the second attempt I added dropped more columns in order to take out some non-essential data, added more neurons and layers and used different activiation functions for the layers. That brought up the accuracy to around 78%.

![Alt text](Starter_Code/Code_Snippet/final_neural_network.png)


Summary:
After making some tweaks in order to optimize the model, I was able to achieve a model performance that was satisfactory. Using this neural network should provide highly accurate results. There are more tweaks that could be made in order to improve the accuracy of the model. One recommendation would be to include even more layers which will familiarize the model to new data. However, adding too many layers could introduce overfitting and slow down the computational speed.
