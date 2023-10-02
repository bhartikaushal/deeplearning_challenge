# deeplearning_challenge

Alphabet Soup is a non-profit organization. This project aims to use neural networks and machine learning models to create a binary classifier to predict if the applicant will succeed if funded by this organization. A CSV file provided by Alphabet Soup containing information on over 34000 applicants was used for this project. 
# Steps Taken

 ## DATA PREPROCESSING:
 1. The dataset was checked for null and duplicate values.
 2. EIN and Name columns were dropped as they are unnecessary for analysis.
   <img width="421" alt="image" src="https://github.com/bhartikaushal/deeplearning_challenge/assets/124011061/bd108fba-7fb6-4dc6-bf10-6be43f1cdc22">

 3. Created a cutoff point to bin "rare" categorical variables in a new value, Other, for CLASSIFICATION and APPLICATION_TYPE.
    <img width="530" alt="image" src="https://github.com/bhartikaushal/deeplearning_challenge/assets/124011061/151826bf-2c05-46cc-a7fc-4e5e2d9daa13">

 4. Converted categorical data to numeric with pd.get_dummies, split the preprocessed data into features and target arrays, then lastly split into training and testing datasets
<img width="347" alt="image" src="https://github.com/bhartikaushal/deeplearning_challenge/assets/124011061/1b3530ac-d26e-4abe-8bf5-6c318420faf0">
<img width="400" alt="image" src="https://github.com/bhartikaushal/deeplearning_challenge/assets/124011061/05a68c23-fd24-481f-946e-f0fc384c9c50">


 5. Target Variable for the model: IS_SUCCESSFUL
    
Feature Variables for the model:

APPLICATION_TYPE
AFFILIATION
CLASSIFICATION
USE_CASE
ORGANIZATION
STATUS
INCOME_AMT
SPECIAL_CONSIDERATIONS
ASK_AMT
## Compiling, Training, and Evaluating the model

I built a model using the Keras library. I added an input layer and used the Relu activation function for the first hidden layer. I used the sigmoid function for the output layer. I did not reach the target accuracy of 75% with this model.
<img width="567" alt="image" src="https://github.com/bhartikaushal/deeplearning_challenge/assets/124011061/c9ffcaf8-7717-439b-b8dd-abc408d05da8">


I optimized the model using different activation functions( LeakyReLU and tanh) for the hidden layers and changed the neuron units, but it did not improve the model's efficiency.
<img width="578" alt="image" src="https://github.com/bhartikaushal/deeplearning_challenge/assets/124011061/6d919285-b8ab-4133-ac58-f04ff26fa442">
<img width="476" alt="image" src="https://github.com/bhartikaushal/deeplearning_challenge/assets/124011061/48003694-cadd-42e3-9af5-dbb7dac60a59">




