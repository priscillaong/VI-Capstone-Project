# VI-Capstone-Project

# Project Statement
The aim of this project is to use historical bank loan data to predict a client's ability to repay future loans based on client's info and credit history.

# Summary of Results
The aim of the project was to use historical bank loan data to predict a client's ability to repay future loans based on client's info and credit history.<br>
Data cleansing was performed on the dataset along with analysis of the data distribution pattern. String type data was mapped to numerical value before finding correlation of different variables with the target. Credit Score, Current Loan Amount and Term were most closely related to the target (Loan Status), of which Credit Score shows the strongest correlation at 0.40.<br>
Before building the Logistic Regression Baseline Model, apart from the assigning of string type data to a numerical value, the numerical data was also normalized.<br>
The Logistic Regression Model did considerably well with an test accuracy of ~0.80 and AUC score of ~0.75. However, upon further analysis via the Confusion Matrix, it was made aware that the number of false positives are high and account for almost all the ~0.20 inaccuracies score in test result.<br>
The KNearest Neighbours and Decision Trees model had test accuracies of ~0.71. Upon applying Grid Search to find the optimal number of neighbours for the KNearest Neighbours model, the test accuracy was improved to ~0.79. However, when evaluating the model, the AUC score was ~0.72 and while the number of false positives decreased slightly, it was compensated with the increase in number of false negatives.<br>
Overall, the performance of both the Logistic Regression and KNearest Neighbours models are about the same. However, it is necessary to improve the accuracy scores of either model and reduce the number of false positives so that the bank would not suffer losses from charged off debts. A balance between the number of false positives and false negatives with a higher accuracy score would be more desirable in this scenario.<br>
Limitations: About 4 columns in the dataset had between 4-53% of null values. It would be good if these values could be provided for better analysis and model prediction. Some other client info such as liquid assets and value of collaterals could be provided for better data analysis and modelling.
