# Package import
## Difference Between `import` and `from ... import` Syntax 

1.import --> This brings in the entire library and gives it a short nickname (pd).
2.from.. import --> This pulls in only one specific class/function directly, so you can call it without the full path.

# Preprocessing

🛠️ Preprocessing Steps for Linear Regression
# Data Cleaning

Handle missing values (drop rows, fill with mean/median, or impute).

Remove duplicates.

Fix data types (e.g., convert strings to numeric where needed).

# Exploratory Data Analysis (EDA)

Use df.describe() and df.info() to understand distributions.

Plot histograms, scatter plots, and correlation heatmaps.

# Feature Scaling

Linear regression is sensitive to scale.

Apply Standardization (Z‑score) or Normalization (Min‑Max) if features vary widely.

Encoding Categorical Variables

Convert categorical features into numeric using One‑Hot Encoding (pd.get_dummies() or sklearn.preprocessing.OneHotEncoder).

# Train/Test Split

Always split data into training and testing sets (e.g., 80/20) using train_test_split.


🎯 How to Select Features

# Domain Knowledge

Think logically: e.g., in housing prices, features like number of rooms, location, and income level matter more than random IDs.

# Correlation Analysis

Use df.corr() or a heatmap to check which features are strongly correlated with the target.

Drop features with very low correlation.

# Multicollinearity Check

If two features are highly correlated with each other (e.g., rooms and house size), keep one to avoid redundancy.

Use Variance Inflation Factor (VIF) to detect multicollinearity.

# Feature Importance

Train a simple model and check coefficients.

Or use feature selection methods like:

Recursive Feature Elimination (RFE).

SelectKBest with statistical tests.