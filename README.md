**Porter** is India's Largest Marketplace for Intra-City Logistics. Leader in the country's $40 billion intra-city logistics market, Porter strives to improve the lives of 1,50,000+ driver-partners by providing them with consistent earning & independence. Currently, the company has serviced 5+ million customers

Porter works with a wide range of restaurants for delivering their items directly to the people.

Porter has a number of delivery partners available for delivering the food, from various restaurants and wants to get an estimated delivery time that it can provide the customers on the basis of what they are ordering, from where and also the delivery partners.

This dataset has the required data to train a regression model that will do the delivery time estimation, based on all those features.

**Data Dictionary**

Each row in this file corresponds to one unique delivery. Each column corresponds to a feature as explained below.
1. market_id : integer id for the market where the restaurant lies
2. created_at : the timestamp at which the order was placed
3. actual_delivery_time : the timestamp when the order was delivered
4. store_primary_category : category for the restaurant
5. order_protocol : integer code value for order protocol(how the order was placed ie: through porter, call to restaurant, pre booked, third part etc)
6. total_items subtotal : final price of the order
7. num_distinct_items : the number of distinct items in the order
8. min_item_price : price of the cheapest item in the order
9. max_item_price : price of the costliest item in order
10. total_onshift_partners : number of delivery partners on duty at the time order was placed
11. total_busy_partners : number of delivery partners attending to other tasks
12. total_outstanding_orders : total number of orders to be fulfilled at the moment

**Process**
1. Import the data and understand the structure of the data:
	• usual exploratory analysis steps like checking the structure & characteristics of the dataset
2. Data preprocessing
	• Cleaning of data
	• Feature engineering: Creating the target column time taken in each delivery from order timestamp (created_at) and delivery timestamp (actual_delivery_time)
	• Getting hour of day from the order time and also the day of the week
	• Understanding pandas datetime data type and what function it provides by default
	• Get delivery time in minutes
3. Handling null values
4. Encoding categorical columns
5. Data visualization and cleaning
	• Visualize various columns for better understanding Countplots, scatterplots
6. Check if the data contains outliers
	• Removing outliers by any method
	• Plotting the data again to see if anything has improved
7. Split the data in train and test
8. Scaling the data for neural networks.
9. Creating a simple neural network
	• Trying different configurations
	• Understanding different activation functions, optimizers and other hyperparameters.
10. Training the neural network for required amount of epochs
11. Plotting the losses and checking the accuracy of the model
12. Checking its various metrics like MSE, RMSE, MAE

**Evaluation Criteria (100 Points):**

1. Defining problem statement, importing the data and data structure analysis (10 points)
2. Data preprocessing and feature engineering (30 points)
	• Data cleaning
	• Null value handling
	• Creating the target column (time taken for delivery) from order timestamp and delivery timestamp
	• Getting hour and day of the week
	• Encoding categorical column
3. Data visualization and cleaning (20 points)
	• Visualization for various features
	• Check for outliers
	• Remove outliers
	• Compare plots and results
4. Regression with neural networks (40 points)
	• Data splitting
	• Data scaling
	• Defining NN architecture
	• Trying different combinations and hyperparameters
	• Model training

**Leading Questions:**

1. Defining the problem statements and where can this and modifications of this be used?
2. List 3 functions the pandas datetime provides with one line explanation.
3. Short note on datetime, timedelta, time span (period)
4. Why do we need to check for outliers in our data?
5. Name 3 outlier removal methods?
6. What classical machine learning methods can we use for this problem?
7. Why is scaling required for neural networks?
8. Briefly explain your choice of optimizer.
9. Which activation function did you use and why?
10. Why does a neural network perform well on a large dataset?
