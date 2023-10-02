# LogisticsRegressionModel
This is a classification on car dataset using logistic regression model.
I renamed the MSRP column to PRICE , the automatic transmission type was most frequent in the column . In the numerical features highway_mpg and city_mpg has the highest correlation .
I made price binary and named it above average when is 1 when it's above mean and 0 other wise 
I  split the  data into train/val/test sets with 60%/20%/20% distribution.
Using Scikit-Learn for the (the train_test_split function) and set the seed to 42. I made sure that the target value (above_average) is not in your dataframe. Afternoon calculating the mutual information between above average and other categorical variables in the dataset, transmission type has the lowest mutual information. Using Scikit-Learn, fitting the model with these parameters:
model = LogisticRegression(solver='liblinear', C=10, max_iter=1000, random_state=42) and rounding the accuracy score to 2 decimal digit the accuracy score is 94%.
