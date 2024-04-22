
Introduction:

This project is aimed at building a propensity model to identify potential customers.

Propensity modeling is a sophisticated technique designed to predict the likelihood of individuals, leads, and customers engaging in specific actions. Leveraging advanced statistical analysis, this methodology meticulously considers both independent variables and confounding factors that influence customer behavior.


Data:

The insurance company has provided with a historical data set (train.csv). The company has also provided with a list of potential customers to whom to market (test.csv). From this list of potential customers, we need to determine yes/no whether the compan
y wishes to market to them. 

Steps involved towards attempting to solve this problem statement: 

•	Exploratory Data Analysis: Analyze and understand the data to identify patterns, relationships, and trends in the data by using Descriptive Statistics and Visualizations. 
•	Data Cleaning: This includes standardization, handling the missing values and outliers resolution in the data. 
•	Dealing with Imbalanced data: This data set is highly imbalanced. The data is balanced using the SMOTEENN technique before moving into model building.
•	Feature Engineering: As provided data shows pdays and pmonths i.e campaign client wast previously contacted, is then featured into categorical column. 
•	Model Selection:  The Problem statement presents a classification task whether to market campaign or not (yes/no).For this purpose  Random Forest Classifier and Support vector machine classifiers are 
        choosen and then ensemble the classifiers with hard probability voting. 
•	Model Training: Splited the data into train & test sets and use the train set to estimate the best model parameters. 
•	Model Validation: Evaluated the performance of the model on data that was not used during the training process. The goal is to estimate the model's ability to generalize to new,unseen data and to identify 
        any issues with the model, such as overfitting. For this purpose Cross validation with 5 folds is used.
•	Model Deployment: Model deployment is the process of making a trained machine learning model available for use in a production environment. 
        A seperate file contains the Source pipeline for model deployment.

Pointers:
Added a column to the test_with.predictions.csv file. In this column, for each observation indicate a yes or a no whether company wishes to market to that candidate.

Metrics Performance:
•	The accuracy of the model on the test data set is  86% .
	Added methods for Hyperparameter tuning.
        Performed model validation. 
Instructions:
- propensify_train.xlsx: Training dataset containing historical data.
- propensify_test.xlsx: Test dataset used to evaluate the model's performance.
- Shivam_Namdeo_Capstone_Project_Propensity model to identify potential customers.ipynb: Jupyter Notebook detailing the model building process.
- Shivam_Namdeo_Source_code_pipeline.ipynb: Notebook containing the code pipeline for data preprocessing and model training.
- propensity_model.joblib: Serialized version of the trained model.
- Preprocessing_pipeline.joblib: Serialized preprocessing pipeline for preparing new data.
