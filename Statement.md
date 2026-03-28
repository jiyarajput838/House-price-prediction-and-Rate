PROJECT TITLE: HOUSE PRICE PREDICTION AND RATE ANALYSIS                        


# 1. Problem statement
<br>House prices in California are different in every area.
<br>They depend on things like:
*	How much people earn in that area (median income)
*	How many rooms houses have
*	How crowded the area is (population, people per house)
* Where the area is on the map (latitude and longitude).It is hard for a normal person to look at all this data and guess a fair house price.

# 2. Scope of the project
This project is small and focused. It does not try to cover everything in real estate. It does only these main things:
*	Uses the California Housing Dataset from scikit-learn (already cleaned and ready). 
*	Works only on one target: median house value of a district (in $100,000 units).
*	Uses 8 numeric inputs: income, house age, average rooms, average bedrooms, population, average occupancy, latitude, longitude.
*	Builds one regression model (Linear Regression) to learn the relationship between these inputs and price.
*	Evaluates the model using RMSE and R², and shows graphs and sample predictions.
This is an academic/learning project, not a real-time app for buying/selling actual houses. It is perfect for a college assignment or mini project.

# 3. Target user
Who can use or benefit from this project?
*	Students 
o	Learning Python and machine learning basics.
o	Want a clear example of a full ML pipeline: load → preprocess → train → evaluate → visualize.
*	Teachers / Project guides
o	Can use it to check if the student understands regression, evaluation metrics, and basic data analysis.
*	Beginners in data science
o	Want to see how simple models like Linear Regression can predict a real-world value (house price) using real data.
This project is not made for real customers or companies, but mainly for learning, teaching, and demonstration.

# 4. High-level features 
Your code has some clear, simple features:
# 1.	Loads data automatically
o	Uses fetch_california_housing() to get the dataset directly from scikit-learn (no manual file download).
# 2.	Shows basic price information
o	Prints minimum, maximum, average, median, 25% and 75% house prices (in dollars).
o	This helps understand the overall price range in California.
# 3.	Builds a regression model
o	Splits data into training and test sets (80% train, 20% test).
o	Scales features using StandardScaler.
o	Trains a LinearRegression model on the training data.
# 4.	Evaluates how good the model is
o	Calculates RMSE (average error in dollars) and R² score (how much variation is explained).
o	Prints something like: RMSE=$53000 | R²=0.57, which is easy to talk about in viva.
# 5.	Visualizes the results
o	Scatter plot: Actual vs Predicted prices (good points lie near the diagonal line).
o	Histogram: Distribution of all house prices (how many houses in each price range).

