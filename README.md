# House-price-prediction-and-Rate
PROJECT TITLE: HOUSE PRICE PREDICTION AND RATE ANALYSIS                        


# 1. Overview
This project predicts median house prices in California using a Linear Regression model.
<br>The dataset comes from the California housing dataset in scikit-learn, which contains information such as median income, average number of rooms, population, and geographic location (latitude and longitude) for different districts in California.
<br>The Python script:
* Loads the dataset
*	Trains a regression model
*	Evaluates it using RMSE and R²
*	Visualizes predictions and price distribution
*	Prints sample predictions with errors

# 2. Features
*	Automatic data loading
o	Uses fetch_california_housing() from scikit-learn (no manual CSV download needed).
*	Price statistics
o	Prints minimum, maximum, average, median, 25th percentile, and 75th percentile of house prices (in dollars).
*	Regression model
o	Uses Linear Regression to predict median house value (in units of $100,000).
*	Feature scaling
o	Uses StandardScaler so that features like income and latitude are on comparable scales.
*	Model evaluation
o	Calculates RMSE (Root Mean Squared Error) and R² score on the test set.
o	Shows how well the model fits the data.
*	Visualizations
o	Scatter plot of Actual vs Predicted prices (with a diagonal reference line).
o	Histogram showing the distribution of all house prices.
*	Sample predictions
o	Prints 5 random examples from the test set with:
*	Actual price
*	Predicted price
*	Absolute error

# 3. Technologies and tools used
*	Programming language: Python 3.x
*	Libraries:
o	numpy – numeric computations
o	matplotlib – plotting graphs
o	scikit-learn –
*	fetch_california_housing (dataset)scikit-learn
*	train_test_split (splitting data)realpython
*	StandardScaler (feature scaling)
*	LinearRegression (regression model)
*	mean_squared_error, r2_score (metrics)
*	Dataset: California Housing dataset (20,640 samples, 8 numerical features, 1 target).

# 4. Steps to install and run the project
# 4.1. Prerequisites
*	Python 3.8 or above installed.scikit-learn
*	pip working in your terminal/command prompt.
# 4.2. Install required libraries
Open Terminal / CMD and run:
bash
pip install numpy matplotlib scikit-learn
This will install NumPy, Matplotlib, and scikit-learn.scikit-learn
# 4.3. Save the project file
<br>1.	Create a new file named, for example, house_price_prediction.py.
<br>2.	Paste your full code into this file.
# 4.4. Run the script
In the terminal, go to the folder where the file is saved:
Then run:
python house_price_prediction.py

# 5. Instructions for testing
When you run the script, it will automatically perform testing on the test set created by train_test_split.realpython
What to look for in the output:
* 1.	Price statistics
o	Check the printed values for:
*	Min price
*	Max price
*	Average price
*	Median
*	25th percentile
8	75th percentile
o	This tells you the approximate price range in the dataset.
* 2.	Model performance (RMSE and R²)
o	The script prints something like:
text
Model: RMSE=$53000 | R²=0.57
o	RMSE (in dollars) shows the average prediction error.
o	R² shows how much of the variation in prices is explained by the model (closer to 1 is better).
* 3.	Plots
o	A window will show two plots:
*	Left plot: Scatter plot of Actual vs Predicted.
*	Points close to the diagonal red line mean good predictions.
*	Right plot: Histogram of all house prices.
*	Shows how many houses are in each price range.
* 4.	Sample predictions
o	At the end, the script prints 5 lines like:
text
House 1: Actual=$180000 | Pred=$200000 | Error=$20000
o	This helps you manually see how close predictions are to real prices.
