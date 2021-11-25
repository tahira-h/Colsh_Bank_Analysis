# Colsh_Bank_Analysis

### Instructions:
You need to apply different classification model for the prediction and find out the better accuracy.

### Language: 
Python

### Tools: 
Excel

### Overview

#### Purpose:

The purpose of this analysis is to use the dataset from a bank services company called Colsh Tech. The dataset from this company will allow analysts to use algorithms to apply different classification model for the prediction and find out the better accuracy. 

### Results

#### Dataset Analysis:

For this analysis, "Train.csv" is the dataset used to complete predictions and find accuracy.

As shown in the image below, the "data" represents all of the feature names(columns) listed in the dataset. There are 13 feature names listed in the dataset: Loan_ID, Gender, Married, Dependents, Education, Self_Employed, ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Property_Area, and Loan_Status.

There is one "target" in the data set, Loan_Status. The Loan_Status column represents individuals listed in the dataset that does or does not have a loan with the bank. In the dataset, "Y" represents individuals that does have a loan, and "N" represents individuals that does not have a loan. 

Open the file containing data_target.

![data_target](/ColshBankAnalysis/Images/data_target.png)
Close the file.

Open the file containing data_set.

![data_set](/ColshBankAnalysis/Images/data_set.png)
Close the file.

  
  
#### Training and Testing:
  
The data is split into training and testing to receive the actual and predicted values.

Open the file containing training_and_testing.

![training_and_testing](/ColshBankAnalysis/Images/training_and_testing.png)
Close the file.



#### Decision Tree Classifier:

After receiving the actual and predicted values, the DecisionTreeClassifier model is imported and accuracy is calculated. According to the accuracy, there are 21 data points missed, providing the wrong calculations. The accuracy percentage is 79%(0.79).

Open the file containing decision_tree_classifier.

![decision_tree_classifier](/ColshBankAnalysis/Images/decision_tree_classifier.png)
Close the file.



#### RandomForestClassifier:

Once the second model, RandomForestClassifier, is imported and the confusion matrix is completed, take a look at the previous accuracy of the first model DecisionTreeClassifer. There were 21 mistakes made with an accuracy score of 79%(0.79). Currently, the RandomForestClassifier has 18 mistakes made with an accuracy score of 82%(0.82). There were 21 mistakes in DecisionTreeClassifer, now the mistakes decreased to 18. 

Open the file containing random_forest_classifier.

![random_forest_classifier](/ColshBankAnalysis/Images/random_forest_classifier.png)
Close the file.



As shown in the image above, Classification Report results for the RandomForestClassifier model shows an accuracy of 82%(0.82), the precision of No for 'Loan_Status' is 85%(0.85), and the recall 
of No for 'Loan_Status' is 49%(0.49). The precision of Yes for 'Loan_Status' is 82%(0.82), and the recall of Yes for 'Loan_Status' is 96%(0.96).


#### Tree Graph:

A decision tree graph is presented showing .png format. The decision tree graph presents results from the dataset. The decision tree includes gini, samples, values, and class. 

As shown in the image below, each box contains characteristics representing the dataset presented in this analysis. The top box(root node) is where a question is asked. The answers for the root node is True and False. If the answer to the root node is True, the action of the question divides the data into smaller subsets. 

Open the file containing decision_tree_graph.

![decision_tree_graph](/ColshBankAnalysis/Images/decision_tree_graph.png)
Close the file.



The root node, Loan_ID_LP001708, has a gini of 0.431, samples is 234, value is 113 and 247, and class is N. 

The root node's results of True gini is 0.425 and False gini 0.0. The results measures the probability of a wrongly classified variable when chosen randomly in this analysis. 

The results of True samples is 233 and False samples is 1. 

The results of True value is 109, 247 and False value is 4, 0. Value is how the tested information is split up. For instance, the root node value is 360, altogether the True value is 356, and altogether the False value is 4.

The results of True class is N, and False class is Y. Whis is the target feature. 

### Summary

#### Results:

The performance of two models DecisionTreeClassifier and RandomForestClassifier were used for the prediction of a dataset provided by bank services company Colsh Tech.
The accuracy rate of the DecisionTreeClassifier model provided wrong calculations of 21 data points missed, and a lower accuracy score of 79%(0.70). In contrast, the accuracy rate of the RandomForestClassifier model provided wrong calculations of 18 data points missed, and a higher accuracy score of 82%(0.82).

#### Recommendation:

With RandomForestClassifier model having the highest percentage score of accuracy. It is recommended that bank services company Colsh Tech use the RandomForestClassifier model to present the better accuracy score for clients listed in the dataset.
