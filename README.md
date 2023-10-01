# deeplearning_challenge

Alphabet Soup is a non-profit organization. This project aims to use neural networks and machine learning models to create a binary classifier to predict if the applicant will succeed if funded by this organization. A CSV file provided by Alphabet Soup containing information on over 34000 applicants was used for this project. 
# Steps Taken

 ## DATA PREPROCESSING:
 1. The dataset was checked for null and duplicate values.
 2. EIN and Name columns were dropped as they are unnecessary for analysis.
 3. Created a cutoff point to bin "rare" categorical variables in a new value, Other, for CLASSIFICATION and APPLICATION_TYPE.
 4. Converted categorical data to numeric with pd.get_dummies, split the preprocessed data into features and target arrays, then lastly split into training and testing datasets
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
