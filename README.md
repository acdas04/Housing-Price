# Housing Price Prediction

## Description
This project aims to predict housing prices based on the area of the house. By using linear regression, the model learns the relationship between the area of a house and its price. This project covers data loading, preprocessing, visualization, model implementation, and evaluation.

## Project Details

### 1. Importing Libraries
We start by importing necessary libraries such as `numpy`, `pandas`, and `matplotlib`.

### 2. Loading and Describing Dataset
We load the dataset using `pandas` and display the basic statistics of the dataset including count, mean, standard deviation, min, 25th percentile, 50th percentile, 75th percentile, and max values for each column.

### 3. Creating Training Set
We extract the input variable (area) and the target variable (price) from the dataset and convert them into numpy arrays for easier manipulation.

### 4. Normalizing the Values
To make the training process more efficient, we normalize the area and price values by dividing them by 1000 and 10000, respectively.

### 5. Visualizing Data
We plot the normalized data points using `matplotlib` to get an initial understanding of the data distribution.

### 6. Model Function
We define the model function `our_model(w, b, x)` that computes the predicted price based on the input area (x), weight (w), and bias (b).

### 7. Cost Function
The cost function `cost_function(x_train, y_train, w, b)` calculates the mean squared error between the predicted prices and the actual prices.

### 8. Gradient Computation
The gradient function `gradient(x_train, y_train, w, b)` computes the gradients of the cost function with respect to the weight and bias.

### 9. Gradient Descent Algorithm
The `gradient_descent_algorithm(x_train, y_train, w_init, b_init, learning_rate, num_iters)` function iteratively updates the weight and bias to minimize the cost function. It also keeps track of the cost function value and the parameters at each iteration.

### 10. Running the Model
We initialize the parameters, run the gradient descent algorithm, and visualize the final model's predictions against the actual data points.

### 11. Results
The final model's predictions are plotted alongside the actual data points. The model can be used to predict the price of a house given its area. For example, the predicted price for a house with 1200 sqft area is printed.

## Installation

To run this project, you need to have Python installed along with the following libraries:
- numpy
- pandas
- matplotlib

You can install these libraries using pip:

```bash
pip install numpy pandas matplotlib

## Example
For a house with a 1200 sqft area, the predicted price is printed and plotted alongside the actual data points.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
