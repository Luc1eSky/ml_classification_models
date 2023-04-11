# Homework Building Classification Models
Homework for class MSDS-599 - build classifiers using different ML models on a synthetically generated data set

Models include:
- K-nearest Neighbor
- Decision Tree Classifiers
-   Bagging 
-   Random Forest
-   Boosting

In the folder is a file called classify_me.csv. The column 'Target' gives the class labels.

1. Read in this file. How many classes are there? How many features are there? Are there any missing entries? 

2. Split into training and test sets (30% test set). Use random_state=5 so your splits are reproducible. 

3. Use all the features to build a classifier on the training set. Try bagging, random forest, boosting, and k-nearest neighbors. For knn, cross validate the number of neighbors you use. In your random forest implementation, build the trees deep -- that is, do not set a value for max_depth. For bagging and random forest,  cross validate the number of trees you use (given by the n_estimators parameter). For your boosting model, validate all of the parameters: n_estimators, learning_rate, and max_depth. In all three models, set random_state=5 so the results are reproducible.  

4. Comment on which model gives the best results on the test set.  For the best model, comment on feature importances (if relevant). 
