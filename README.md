# Classification-of-APS-Failure-data-using-Decision-Trees
The dataset is obtained from - https://archive.ics.uci.edu/ml/datasets/APS+Failure+at+Scania+Trucks

The first step was the pre-processing stage where missing data was filled using the mean of the remaining elements in the column. 
Next, the coefficient variation for 170 features was calculated and only the square root of 170 features was analysed to visualise the dataset.
The original imbalanced dataset was first trained by a random forest classifier which gave an AUC curve value of 0.8594. Then SMOTE was applied to remedy class imbalance, this gave a AUC curve value of 0.9136. 

As it can be seen, the results are much better when SMOTE is applied to handle imbalanced classes. 

Next, the Logistic Model Trees were trained when WEKA was called on Scikit Learn. In the case of unbalanced dataset, based on the confusion matrix, we can see that a classification tree provided better results compared to a regression tree on the test dataset. Whereas, in the case of a balanced dataset, a logistic model tree performance was better than the classification tree performance. 
