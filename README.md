# Analyzing-Airbnb-Listings-Data



DATASET LINK:https://www.kaggle.com/datasets/arianazmoudeh/airbnbopendata



This code analyzes Airbnb listings data to extract insights and build a predictive model for the price of a listing based on its features.

The code first loads the Airbnb listings data into a Pandas DataFrame and then drops unnecessary columns. It then checks for missing values and drops rows with missing values for the 'last_review' column. The code fills in missing values for the 'reviews per month' column with the mean value and drops any duplicate rows. Finally, it exports the cleaned dataset to a new CSV file.

The next section of the code reads in the cleaned CSV file and cleans up the 'price' column by removing dollar signs and commas and converting it to a float data type. It calculates the mean price across all listings and calculates the mean price and number of listings in each neighborhood. It then creates a bar chart of mean price by neighborhood to visualize the results.

The final section of the code prepares the data for a linear regression model to predict the price of a listing based on its features. It drops rows with missing values in the target variable ('price') and defines the target variable and features. It uses one-hot encoding to convert the 'room type' feature into numerical values and imputes missing values in the features using the median. It also removes the '$' sign from the target variable and converts it to float values. It then splits the data into training and testing sets, trains the linear regression model, predicts on the test set, and evaluates the model's performance using root mean squared error. The code prints the shape of the input data and target variable and the root mean squared error of the model.





