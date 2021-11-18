# House-Prices-Advanced-Regression-Techniques


We choose to work on the Colab notebooks environment.
The project provides us with two inputs as two datasets. One is called ‘train_data’ which will be used to train model; The other is called ‘test_data’ which will be used as the dataset to test our model and to make the prediction. In this project First we applied Simple linear regression with multiple variables , then we try to improve the result and we did more analysis to the dataset And  applied regression teqnieqes see the effect on the result or not.
we will try to predict the house prices for 1459 houses in the test dataset. We vertical stacking of GBoost, LightGBM, and Lasso.



Data Exploration
Data Exploration is the key to getting insights from data. Practitioners say a good data exploration strategy can solve even complicated problems in a few hours. A good data exploration strategy comprises the following:

Univariate Analysis - It is used to visualize one variable in one plot. Examples: histogram, density plot, etc.
Bivariate Analysis - It is used to visualize two variables (x and y axis) in one plot. Examples: bar chart, line chart, area chart, etc.
Multivariate Analysis - As the name suggests, it is used to visualize more than two variables at once. Examples: stacked bar chart, dodged bar chart, etc.
Cross Tables -They are used to compare the behavior of two categorical variables.














2. Problem Statement
Predict the sale price of houses in Ames, Iowa, given 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, to predict the final price of each home.
 3. Used Dataset.
The data set used in this project describes the sale of individual residential property in Ames, Iowa from 2006 to 2010. The data set contains 2930 observations and a large number of explanatory variables (23 nominal, 23 ordinal, 14 discrete, and 20 continuous) involved in assessing home values.






We import both the "train" and "test" dataset.
*As we can see, the Training dataset has 1460 observations and 81 columns, while the Test dataset has 1459 observations and 80 columns (since it's missing the target variable).


We use the ‘read.csv’ syntax in R to read in these two datasets.
After a quick scan of these two datasets, we choose to combine these two datasets together, even if they will be used in different ways, just because we want to clean the whole data firstly. We delete the column ‘Id’ both in train and test and delete the column ‘SalePrice’ in train which is our target variable and does not appear in test dataset. Now there are 78 variables remained in the combined dataset called ‘df.combined’.
