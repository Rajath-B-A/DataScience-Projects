
## Problem Statement 

Porter works with a wide range of restaurants for delivering their items directly to the people. Porter has a number of delivery partners available for delivering the food, from various restaurants and wants to get an estimated delivery time that it can provide the customers on the basis of what they are ordering, from where and also the delivery partners. Using the data train a NN regression model that will do the delivery time estimation, based on all the features.


## Process

Import the data and understand the structure of the data: • usual exploratory analysis steps like checking the structure & characteristics of the dataset
Data preprocessing • Cleaning of data • Feature engineering: Creating the target column time taken in each delivery from order timestamp (created_at) and delivery timestamp (actual_delivery_time) • Getting hour of day from the order time and also the day of the week • Understanding pandas datetime data type and what function it provides by default • Get delivery time in minutes
Handling null values
Encoding categorical columns
Data visualization and cleaning • Visualize various columns for better understanding Countplots, scatterplots
Check if the data contains outliers • Removing outliers by any method • Plotting the data again to see if anything has improved
Split the data in train and test
Scaling the data for neural networks.
Creating a simple neural network • Trying different configurations • Understanding different activation functions, optimizers and other hyperparameters.
Training the neural network for required amount of epochs
Plotting the losses and checking the accuracy of the model
Checking its various metrics like MSE, RMSE, MAE 
Dataset: https://d2beiqkhq929f0.cloudfront.net/public_assets/assets/000/015/039/original/dataset.csv.zip?1663710760

## Data Dictionary

Each row in this file corresponds to one unique delivery. Each column corresponds to a feature as explained below.

market_id : integer id for the market where the restaurant lies 
created_at : the timestamp at which the order was placed 
actual_delivery_time : the timestamp when the order was delivered s
tore_primary_category : category for the restaurant 
order_protocol : integer code value for order protocol(how the order was placed ie: through porter, call to restaurant, pre booked, third part etc) 
total_items subtotal : final price of the order 
num_distinct_items : the number of distinct items in the order 
min_item_price : price of the cheapest item in the order 
max_item_price : price of the costliest item in order 
total_onshift_partners : number of delivery partners on duty at the time order was placed 
total_busy_partners : number of delivery partners attending to other tasks 
total_outstanding_orders : total number of orders to be fulfilled at the moment