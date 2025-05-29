# Task-3-Linear-Regression

# 1. Importing and Preprocessing the Dataset
I began by importing the housing dataset into a pandas DataFrame. To prepare the data for modeling, I converted all categorical variables into numerical form. Specifically, columns with 'yes' and 'no' responses were mapped to 1 and 0, respectively. The 'furnishingstatus' column, which had values like 'unfurnished', 'semi-furnished', and 'furnished', was encoded numerically as 0, 1, and 2. This preprocessing ensured that all features were in a suitable format for machine learning algorithms.

# 2. Splitting Data into Train-Test Sets
After preprocessing, I separated the target variable (house price) from the features. The dataset was then split into training and test sets, with 80% of the data used for training the model and 20% reserved for evaluating its performance. This split helps assess how well the model generalizes to unseen data.

# 3. Fitting a Linear Regression Model
With the data prepared and split, I trained a linear regression model using the training set. The model learned the relationships between the various features (such as area, number of bedrooms, and amenities) and the target variable (price).

# 4. Evaluating the Model
Once the model was trained, I used it to predict house prices on the test set. I evaluated the model's performance using three metrics: Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²). MAE measures the average magnitude of errors in predictions, MSE penalizes larger errors more heavily, and R² indicates the proportion of variance in the target variable explained by the model.

# 5. Plotting the Regression Line and Interpreting Coefficients
To visualize the model, I plotted the regression line showing the relationship between area and price, while keeping other features constant. This helped illustrate how changes in area affect the predicted price according to the model. Additionally, I interpreted the model’s coefficients to understand the impact of each feature on the predicted price. The coefficients represent the expected change in price for a one-unit increase in each feature, holding other features constant. The intercept indicates the predicted price when all features are at their baseline values.