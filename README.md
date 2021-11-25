# Colsh_Bank_Analysis

### Instructions:
You need to apply different classification model for the prediction and find out the better accuracy.

### Languages: 
Python

### Tools: 
Excel

### OVERVIEW

The Purpose

The purpose of this analysis is to use the dataset from a bank services company called Colsh Tech. The dataset from this company will allow analysts to use algorithms to apply different classification model for the prediction and find out the better accuracy. 

The analysis provided will evaluate the performance of the model and recommend whether or not the model should be used to predict better accuracy for the bank clients listed in the dataset.

### RESULTS

Data Set Analysis

For this analysis, "Train.csv" is the dataset used to complete predictions and find accuracy.

There are 13 feature names(columns) listed in this data set. The "data" represent all of the feature names listed from the .csv data set. The feature names are: Loan_ID, Gender, Married, Dependents, Education, Self_Employed, ApplicantIncome, CoapplicantIncome, LoanAmount, Loan_Amount_Term, Credit_History, Property_Area, and Loan_Status.

There is one "target" in the data set, Loan_Status. The Loan_Status column represents individuals in the data set that does or does not have a loan with the bank. In the data set, the "Y" represents individuals with a loan, the "N" represents individuals without a loan. The analysis is to figure out why the Y and N is there. 

  ----------------data_target pic here---------------


Decision Tree Classifier

For the Native Random Oversampling data, results shows that the balanced accuracy test is 64.94%(0.6494575410534504), the precision is 1%(1.00), and the recall is 73%( 0.73).


Classification Report
	(Line 114)... Line 113 too??

For the first Classification Report completed after the Decision Tree Classifier, 
results show that the accuracy is 82%(0.82),
the precision of No for 'Loan_Status' is 85%(0.85), and the recall 
of No for 'Loan_Status' is 49%(0.49),
the precision of Yes for 'Loan_Status' is 82%(0.82), and the recall
of Yes for 'Loan_Status' is 96%(0.96).

Confusion Matrix
...

Classification Report 
	(LINE 117)


For the first Classification Report completed after the confusion matrix was 
completed, the Classification Report 
shows accuracy increased to 83%(0.8333333333333334),
the precision of No for 'Loan_Status' is 86%(0.86), and the recall 
of No for 'Loan_Status' is 51%(0.51),
the precision of Yes for 'Loan_Status' is 83%(0.83), and the recall
of Yes for 'Loan_Status' is 96%(0.96).

Tree Graph
	(cell "import graphviz")

A tree graph is presented showing .png format. What the graph presents is



Tree Plot
	(cell "fn=train.feature_names")

A tree plot is presented showing .png format. What the graph presents is


### SUMMARY

Results

The Oversampled, Undersampled, and Combination of (Over and Under) 
Sampled data predicted which loans are at higher risk for LendingClub. 
The accuracy rate of the data provided was lower than the data provided 
for Balanced Random Forest Classifier and Easy Ensemble AdaBoost Classifier. 
In addition, the accuracy rate of the data provided from Easy Ensemble 
AdaBoost Classifier was higher than Balanced Random Forest Classifier. 
As aforementioned, Easy Ensemble AdaBoost Classifier data results shows 
that the balanced accuracy test is 91.78%(0.9178773283613644), 
the precision is 1%(1.00), and the recall is 89%(0.89).

Recommendation

With Easy Ensemble AdaBoost Classifier having the highest percentage 
of accuracy score, balance of precision, and recall scores. It is recommended 
that LendingClub uses Easy Ensemble AdaBoost Classifier's data to predict 
credit risk.




=================================================
Video from class

Gini: 
Gini index or Gini impurity measures the degree or 
probability of a particular variable being wrongly classified 
when it is randomly chosen. But what is actually meant by 'impurity'? 
If all the elements belong to a single class, then it can be called pure.


Samples 

Value: 

Class
