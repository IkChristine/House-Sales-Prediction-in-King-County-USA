# House Sales Prediction in King County USA
Data Analysis with Python

This dataset contains house sale prices for King County, which includes Seattle. It includes homes sold between May 2014 and May 2015.

The following questions were explored in this analysis:

## Data Wrangling 

1. Drop the columns "id" and "Unnamed: 0" from axis 1 using the method
drop() , then use the method describe() to obtain a statistical summary of
the data.
2. replace the missing values of the column 'bedrooms' with the mean
of the column 'bedrooms' and 'bathrooms' with the
mean of the column 'bathrooms'using the method replace() .

## Exploratory Data Analysis
3. Use the method value_counts to count the number of houses with unique
floor values, use the method .to_frame() to convert it to a dataframe.
4. Use the function boxplot in the seaborn library to determine whether houses
with a waterfront view or without a waterfront view have more price outliers.
5. Use the function regplot in the seaborn library to determine if the feature
sqft_above is negatively or positively correlated with price.
6. use the Pandas method corr() to find the feature other than price
that is most correlated with price.

## Model Development
7. Fit a linear regression model using the longitude feature 'long' and
caculate the R^2.
8. Fit a linear regression model to predict the 'price' using the feature
'sqft_living' then calculate the R^2.
9. Fit a linear regression model to predict the 'price' using the list of features. Then calculate the R^2. Take a screenshot of your code.
10. Create a list of tuples, the first element in the tuple contains the name of the estimator:
      'scale'
      'polynomial'
      'model'
      The second element in the tuple contains the model constructor
      StandardScaler()
      PolynomialFeatures(include_bias=False)
      LinearRegression()
11. Use the list to create a pipeline object to predict the 'price', fit the object using
the features in the list features , and calculate the R^2.
12. split the data into training and testing sets (test_size=0.1)
13. Create and fit a Ridge regression object using the training data, set the
regularization parameter to 0.1, and calculate the R^2 using the test data.
14. Perform a second order polynomial transform on both the training data and
testing data. Create and fit a Ridge regression object using the training data, set
the regularisation parameter to 0.1, and calculate the R^2 utilising the test data
provided. Take a screenshot of your code and the R^2.
