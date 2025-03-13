# Assignment1_DAI-101
# Melbourne Housing Data Cleaning and Exploratory Data Analysis (EDA)

## Dataset Overview
The **Melbourne Housing dataset** contains real estate data from Melbourne, Australia. The dataset includes details such as property location, price, number of rooms, type, method of sale, and various geographical and structural attributes.

## Data Cleaning Steps
1. **Handling Missing Values:**
   - Columns with a significant amount of missing data were either removed or imputed.
   - Numerical columns such as `BuildingArea`, `Landsize`, and `Price` were imputed using the **median** to avoid skewness.
   - Categorical columns such as `Suburb` were filled using the **mode**.
   
2. **Detecting and Removing Duplicates:**
   - Duplicate rows were identified and removed to maintain dataset integrity.

3. **Fixing Date Formats:**
   - The `Date` column contained inconsistent date formats, which were standardized using `pd.to_datetime()` with the appropriate format.

4. **Standardizing Categorical Values:**
   - Inconsistent category labels (such as typos or mixed letter cases) were standardized.
   - Categories like `Type` (h, u, t) were mapped to their full descriptions (`house`, `unit`, `townhouse`).

5. **Handling Outliers:**
   - Outliers in numerical columns such as `Price`, `Landsize`, and `BuildingArea` were detected using the **Interquartile Range (IQR) method** and either capped or replaced with the median.

## Exploratory Data Analysis (EDA)
1. **Summary Statistics:**
   - Calculated **mean, median, mode, variance, skewness**, and other statistical measures for numerical columns.

2. **Distribution Analysis:**
   - **Histograms and Box Plots** were used to visualize the distribution of `Price`, `Landsize`, and `Rooms`.

3. **Bivariate Analysis:**
   - **Correlation Matrix & Heatmap**: Showed relationships between numerical variables such as `Rooms`, `Price`, `Landsize`, and `PropertyCount`.
   - **Scatter Plots**: Explored relationships like `Price vs. Distance` and `Price vs. Rooms`.
   - **Box Plots & Violin Plots**: Compared categorical variables (`Type`, `Regionname`) with numerical values like `Price`.

## Key Observations
- Properties with more rooms and larger land sizes generally had higher prices, as expected.
- **Price and Distance from the city center showed a weak negative correlation**, meaning properties closer to the city tend to be more expensive.
- Some attributes like `BuildingArea` had significant missing values, making imputation necessary.
- `PropertyCount` values were closely tied to the `Regionname`, indicating region-based differences in housing density.

## Conclusion
Through data cleaning and EDA, the dataset was transformed into a more structured and usable form, removing inconsistencies and identifying key patterns in Melbourne’s real estate market.

---

### Next Steps:
- Perform feature engineering to create new insights.
- Train predictive models for price estimation.
- Conduct time-series analysis to observe market trends over the years.
