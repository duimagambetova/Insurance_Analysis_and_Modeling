# Insurance Data Analysis and Model Evaluation

## Project Overview

This project performs exploratory data analysis (EDA) on an insurance dataset, followed by pre-processing and the application of several machine learning models. The goal is to predict insurance charges based on customer data, using models like Linear Regression, Gradient Boosting, Random Forest, and Polynomial Regression.

## Steps and Methodology

### 1. Data Loading
The insurance dataset is loaded from a CSV file containing information about individuals and their respective insurance charges.

### 2. Exploratory Data Analysis (EDA)
- **Data Types**: We analyze the data types of each column and identify categorical and numerical features.
- **Missing Values**: We check for any missing data in the dataset and handle it if necessary.
- **Duplicate Rows**: Duplicate rows are identified and removed.
- **Descriptive Statistics**: We calculate key statistics (mean, median, standard deviation, etc.) for numerical features.
- **Data Visualizations**: We visualize the distributions of numerical and categorical features to uncover patterns and trends in the data.

### 3. Data Preprocessing
- **Encoding Categorical Variables**: Categorical features like `sex`, `smoker`, `region`, and `children` are encoded to numerical values using `OneHotEncoding` or manual mappings.
- **Feature Scaling**: The numerical features like `age` and `bmi` are scaled using `StandardScaler` to ensure that the models perform optimally.
- **Log Transformation**: A log transformation is applied to the target variable `charges` to handle skewness and make the data more normal.

### 4. Model Training and Evaluation
- **Train-Test Split**: The dataset is split into training and testing sets (80% training and 20% testing).
  
- **Models Used**:
  - Linear Regression
  - Gradient Boosting
  - Random Forest
  - Polynomial Regression
  
- **Model Evaluation**: The models are evaluated based on accuracy, R2 score, mean squared error (MSE), root mean squared error (RMSE), and mean absolute error (MAE).

### 5. Results and Conclusion
- **Best Models**: Gradient Boosting and Polynomial Regression are identified as the best models based on all metrics.
- **Insights**: Gradient Boosting outperforms Polynomial Regression slightly in R2 and MAE.


## Requirements
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scipy`
- `sklearn`

You can install all required libraries by running:

```bash
pip install -r requirements.txt


