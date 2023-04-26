# Parkinson's-Disease-Detection
Trains an SVM (Support Vector Machine) classifier using a dataset containing data on vocal characteristics of people with and without Parkinson's disease
working steps of the project:
* 1.The dataset is read from the "parkinsons.csv" file and assigned to a variable named "data".
* 2.The first five rows of the dataset and its size are displayed. Also, the "isnull()" function is used to check for any missing data and the results are displayed.
* 3.The number of values 0 and 1 in the "status" column of the dataset is counted and displayed using the "value_counts()" function. This is done to determine how many people have Parkinson's disease and how many are healthy.
* 4.The average of characteristics of people with and without Parkinson's disease is displayed, grouped by the "status" column.
* 5.By removing the "name" and "status" columns from the data set, the characteristics assigned to the "X" variable are determined and the disease status is determined with the "status" column assigned to the "Y" variable.
* 6.Using the "train_test_split()" function, the data set is split into training and test sets. The training set is determined as 80% and the test set as 20%.
* 7.The "StandardScaler()" function is used to scale the features. It is applied first on the training set and then on the test set.
* 8.An SVM classifier is trained using "svm.SVC(kernel='linear')".
* 9.In the training set, the accuracy of the model is calculated and displayed using the "accuracy_score()" function.
* 10.In the test set, the accuracy of the model is calculated and displayed using the "accuracy_score()" function.
* 11.A set of property values is generated and using the "predict()" function, it is predicted to which class (with or without Parkinson's disease) these properties belong.
* 12.According to the prediction result, the result is printed.
