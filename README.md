What This Project Does?

This notebook performs the following steps:

1. Data Loading
	•	Imported the California Housing dataset using fetch_california_housing() from sklearn.datasets.
	•	Converted the dataset into a Pandas DataFrame and added the target variable as a new column called Price.

2. Data Cleaning
	•	Replaced any infinite values (inf, -inf) with NaN.
	•	Dropped rows with missing values using dropna().

3. Exploratory Data Analysis (EDA)
	•	Displayed basic statistics and checked for missing values.
	•	Calculated the correlation matrix of all variables.
	•	Used pairplot() from Seaborn to visualize relationships between features.
	•	Created boxplots for detecting outliers in the dataset.

4. Feature Scaling
	•	Applied MinMaxScaler to scale the entire dataset.
	•	Split data into features (independent variables) and target (Price).
	•	Used train_test_split to divide the data into training and testing sets (70/30 split).
	•	Applied StandardScaler for standardizing features.
	•	Replaced any remaining NaN, inf, -inf values with zero using np.nan_to_num().

5. Model Training
	•	Trained a Linear Regression model using sklearn.linear_model.LinearRegression.
	•	Fitted the model on the scaled training data.

6. Model Evaluation
	•	Predicted house prices on the test dataset.
	•	Evaluated the model using:
	•	Mean Squared Error (MSE)
	•	R² Score (Coefficient of Determination)

7. Visualization Output
	•	Saved boxplots for the original dataset, training set, and testing set after scaling as:
	•	boxplot.jpg
	•	boxPlotTrainData.jpg
	•	boxPlotTestData.jpg
