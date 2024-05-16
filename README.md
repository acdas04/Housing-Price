# Housing-Price
This project demonstrates the implementation of linear regression using gradient descent to predict housing prices based on the size of the house. It includes data normalization, cost function computation, gradient computation, and the gradient descent algorithm for parameter optimization.
Project Details
The project is structured as follows:

Importing Libraries
We start by importing necessary libraries such as numpy, pandas, and matplotlib.

Loading and Describing Dataset
We load the dataset using pandas and display the basic statistics of the dataset including count, mean, standard deviation, min, 25th percentile, 50th percentile, 75th percentile, and max values for each column.

Creating Training Set
We extract the input variable (area) and the target variable (price) from the dataset and convert them into numpy arrays for easier manipulation.

Normalizing the Values
To make the training process more efficient, we normalize the area and price values by dividing them by 1000 and 10000, respectively.

Visualizing Data
We plot the normalized data points using matplotlib to get an initial understanding of the data distribution.

Model Function
We define the model function our_model(w, b, x) that computes the predicted price based on the input area (x), weight (w), and bias (b).

Cost Function
The cost function cost_function(x_train, y_train, w, b) calculates the mean squared error between the predicted prices and the actual prices.

Gradient Computation
The gradient function gradient(x_train, y_train, w, b) computes the gradients of the cost function with respect to the weight and bias.

Gradient Descent Algorithm
The gradient_descent_algorithm(x_train, y_train, w_init, b_init, learning_rate, num_iters) function iteratively updates the weight and bias to minimize the cost function. It also keeps track of the cost function value and the parameters at each iteration.

Running the Model
We initialize the parameters, run the gradient descent algorithm, and visualize the final model's predictions against the actual data points.

Results
The final model's predictions are plotted alongside the actual data points. The model can be used to predict the price of a house given its area. For example, the predicted price for a house with 1200 sqft area is printed.

