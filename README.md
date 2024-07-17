# ML-Classifiers
Comparing Classifiers with a banking related dataset.

Business understanding : 
The classification goal is to analyze banking phone calls dataset and predict if the client will subscribe (yes/no) a term deposit (variable y).

Data Understanding : 
The data is related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed. 

There are four datasets: 
1) bank-additional-full.csv with all examples (41188) and 20 inputs, ordered by date (from May 2008 to November 2010), very close to the data analyzed in [Moro et al., 2014]

Data Preparation : 

The dataset is clean with zero nans or missing values. 
Renamed the column names to remove the quotation marks. 
Replaced boolean or simple categorical columns with numeric values wherever possible.
Based on exploratory data analysis, selected these features for the analysis : ['default', 'housing', 'loan', 'duration', 'age', 'job', 'marital'] 
Converted the categorical columns to numerical columns using pd.get_dummies
Split the dataset into Test and Training datasets.

Modeling : 
Scaled the data using Standard Scaler
Built the Logistic Regression, KNN with 5 neighbors, SVC and Decision Tree classification models
Fit the models using the training dataset.

Evaluation : 
