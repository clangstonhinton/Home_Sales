# Home_Sales
Utilize PySpark and Spark SQL on Google Colab, to analyze homes sales data and determine key metrics.

<img width="807" height="600" alt="Screen Shot 2023-05-09 at 12 32 48 PM" src="https://github.com/clangstonhinton/Home_Sales/assets/44728723/cb7876c4-2d19-46d0-9605-a482cc28c6e1">

## Overview of the Analysis
The purpose of this analysis was to build a neural network machine learning model for the nonprofit foundation Alphabet Soup to help it select the applicants for funding with the best chance of success in their ventures. A binary classifer neural network model was built to predict whether applicants will be successful if funded by Alphabet Soup. A target accuracy of 75% was set for the classifer.

### Data Description:
 - The dataset contains information for more than 34,000 organizations that have received funding from Alphabet Soup over the years. The metadata contains 12 columns including: EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, and IS_SUCCESSFUL.

 - The "target" variable for the model is the "IS_SUCCESSFUL" column indicating if the money was used effectively or not. A value of "0" indicates that the grant money was NOT used effectively. A "1" indicates that the grant money WAS used effectively. 

### Approach:
 1. Data Preprocessing:
    - The EIN and NAME colums were removed from the input data as these data were not viewed as targets nor features.
    - For APPLICATION_TYPE and CLASSIFICATION feature columns which have more than 10 unique values, a cutoff point to bin "rare" categorical variables into an "other" category was determine. APPLICATION_TYPE values were cutoff at 500 and CLASSIFICATION values were cut off at 300.
    - The data were split into labels (the predicted target value of "IS_SUCCESSFUL") and features (remaining columns).
    - The data were split into training and testing sets using scikit learn train_test_split function and scaled using StandardScaler.

 2. Original Model Run:  
 An original Neural Network model was compiled, traned and evaluated for accuracy based on the followign parameters.
    - Hidden Layers = 2
    - Number of Nodes in Hidden Layers = 32 nodes each
    - Hidden Layer Activation Function = relu
    - Batch Size = 32
    - Epochs = 30
    - Model Optimizer = adam
    
