
# Data Analysis and Prediction using Python

This project consists of analyzing and predicting housing prices using attributes and features such as square footage, number of bedroom, number of floors, etc. 

The dataset used contains house sale prices for King County, which includes Seattle. It includes homes sold between May 2014 and May 2015.
[Source of the dataset](https://www.kaggle.com/harlfoxem/housesalesprediction?utm_medium=Exinfluencer&utm_source=Exinfluencer&utm_content=000026UJ&utm_term=10006555&utm_id=NA-SkillsNetwork-wwwcourseraorg-SkillsNetworkCoursesIBMDeveloperSkillsNetworkDA0101ENSkillsNetwork20235326-2022-01-01).

# Project Steps

### Importing the Data Sets
- Loading the csv file
- Getting a glimpse of the dataframe
- Displaying the data types of each column using the function dtypes
- Obtaining a statistical summary of the dataframe

### Data Wrangling
- Dropping some columns using the method drop(), then using the method describe() to obtain a statistical summary of the data.
- Checking for missing values
- Replacing the missing values with the mean of the column using the method replace()

### Exploratory Data Analysis
- Using the method value_counts to count the number of houses with unique floor values and the method .to_frame() to convert it to a dataframe
- Using the function boxplot in the seaborn library to determine whether houses with a waterfront view or without a waterfront view have more price outliers
- Using the function regplot in the seaborn library to determine if the feature sqft_above is negatively or positively correlated with price
- Using the Pandas method corr() to find the feature other than price that is most correlated with price

### Model Development
- Fitting a linear regression model using the longitude feature 'long' and caculate the R^2
- Fitting a linear regression model to predict the 'price' using the feature 'sqft_living' then calculate the R^2
- Fitting a linear regression model to predict the 'price' using the list of features
- Creating a list of tuples, the first element in the tuple contains the name of the estimator and the second element contains the model constructor
- Using the list to create a pipeline object to predict the 'price', fitting the object using the features in the list features, and calculating the R^2

### Model Evaluation and Refinement
- Importing the required modules
- Splitting the data into training and testing sets
- Creating and fitting a Ridge regression object using the training data, setting the regularization parameter to 0.1, and calculating the R^2 using the test data
- Performing a second order polynomial transform on both the training data and testing data. Creating and fitting a Ridge regression object using the training data, setting the regularisation parameter to 0.1, and calculating the R^2 utilizing the test data provided.


