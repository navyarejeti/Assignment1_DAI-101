# Assignment1_DAI-101
Data Cleaning and Exploratory Data Analysis (EDA) - Melbourne Housing Dataset

This project involves data cleaning and exploratory data analysis (EDA) on a housing dataset. The goal is to preprocess the dataset by handling missing values, detecting and treating outliers, normalizing categorical values, and analyzing relationships between different variables.

Data Cleaning Steps

Handling Missing Values
Numerical missing values were filled using the median (skewed data).
Categorical missing values were filled using the mode (most frequent category).
Some missing values in specific columns were inferred based on regional trends.

Fixing Data Inconsistencies
Standardized categorical values by correcting typos and formatting inconsistencies.
Checked for duplicate records and removed them if necessary.

Outlier Detection and Treatment
Used boxplots and IQR (Interquartile Range) method to detect outliers.
Outliers were replaced with the median to maintain data integrity.

Exploratory Data Analysis (EDA)

Summary Statistics
Mean, median, mode, variance, standard deviation, skewness, and kurtosis were calculated to understand data distribution.

Visualizations for Single Variables
Histograms and box plots were used to analyze the distribution of numerical variables.
Bar charts were plotted for categorical variables to observe frequency distributions.

Bivariate Analysis
Correlation matrix & heatmap: Used to identify relationships between numerical variables.
Scatter plots: Explored relationships between variables like Price and Land Size.
Bar plots, violin plots, and box plots: Compared numerical and categorical variables.

Multivariate Analysis
Pair plots: Visualized multiple relationships simultaneously.
Grouped comparisons: Identified combined effects of multiple features like Rooms, Price, and Distance.

Key Observations

Correlation Analysis:
Highly correlated features indicate potential multicollinearity, affecting predictive modeling.
Price and Number of Rooms showed a strong positive correlation.
Latitude and Longitude had no correlation with property price, implying location may need new meaningful variables.

Missing Values & Distribution:
Certain attributes had a high percentage of missing values, which were handled accordingly.
Some categorical variables were imbalanced, requiring sampling adjustments in future modeling.

Outlier Impact:
Large property sizes and extreme prices were identified as outliers.
Imputing extreme values with the median helped stabilize the dataset.
