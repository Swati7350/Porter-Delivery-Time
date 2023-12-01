**Porter** is India's Largest Marketplace for Intra-City Logistics. Leader in the country's $40 billion intra-city logistics market, Porter strives to improve the lives of 1,50,000+ driver-partners by providing them with consistent earning & independence. Currently, the company has serviced 5+ million customers

Porter works with a wide range of restaurants for delivering their items directly to the people.

Porter has a number of delivery partners available for delivering the food, from various restaurants and wants to get an estimated delivery time that it can provide the customers on the basis of what they are ordering, from where and also the delivery partners.

This dataset has the required data to train a regression model that will do the delivery time estimation, based on all those features.
**Data Dictionary**

Each row in this file corresponds to one unique delivery. Each column corresponds to a feature as explained below.

market_id : integer id for the market where the restaurant lies
created_at : the timestamp at which the order was placed
actual_delivery_time : the timestamp when the order was delivered
store_primary_category : category for the restaurant
order_protocol : integer code value for order protocol(how the order was placed ie: through porter, call to restaurant, pre booked, third part etc)
total_items subtotal : final price of the order
num_distinct_items : the number of distinct items in the order
min_item_price : price of the cheapest item in the order
max_item_price : price of the costliest item in order
total_onshift_partners : number of delivery partners on duty at the time order was placed
total_busy_partners : number of delivery partners attending to other tasks
total_outstanding_orders : total number of orders to be fulfilled at the moment
Process

**Import the data and understand the structure of the data:
**
  usual exploratory analysis steps like checking the structure & characteristics of the dataset
  Data preprocessing
  Cleaning of data
  Feature engineering: Creating the target column time taken in each delivery from order timestamp (created_at) and delivery timestamp (actual_delivery_time)
  Getting hour of day from the order time and also the day of the week
  Understanding pandas datetime data type and what function it provides by default
  Get delivery time in minutes
  Handling null values
  Encoding categorical columns
  Data visualization and cleaning
  Visualize various columns for better understanding Countplots, scatterplots
  Check if the data contains outliers
  Removing outliers by any method
  Plotting the data again to see if anything has improved
  Split the data in train and test
  Scaling the data for neural networks.
  Creating a simple neural network
  Trying different configurations
  Understanding different activation functions, optimizers and other hyperparameters.
  Training the neural network for required amount of epochs
  Plotting the losses and checking the accuracy of the model
  Checking its various metrics like MSE, RMSE, MAE
**Evaluation Criteria (100 Points):
**
  Defining problem statement, importing the data and data structure analysis (10 points)
  Data preprocessing and feature engineering (30 points)
  Data cleaning
  Null value handling
  Creating the target column (time taken for delivery) from order timestamp and delivery timestamp
  Getting hour and day of the week
  Encoding categorical column
  Data visualization and cleaning (20 points)
  Visualization for various features
  Check for outliers
  Remove outliers
  Compare plots and results
  Regression with neural networks (40 points)
  Data splitting
  Data scaling
  Defining NN architecture
  Trying different combinations and hyperparameters
  Model training
  Leading Questions:

**Defining the problem statements and where can this and modifications of this be used?
**
  List 3 functions the pandas datetime provides with one line explanation.
  Short note on datetime, timedelta, time span (period)
  Why do we need to check for outliers in our data?
  Name 3 outlier removal methods?
  What classical machine learning methods can we use for this problem?
  Why is scaling required for neural networks?
  Briefly explain your choice of optimizer.
  Which activation function did you use and why?
  Why does a neural network perform well on a large dataset?
