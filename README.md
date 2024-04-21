# Data Cleansing Steps
This README outlines the specific data cleansing steps performed on the dataset.

## Steps
### 1. Removing Duplicate Values
- **Description:** Eliminate duplicate records to ensure data integrity and avoid redundancy.
- **Actions:**
  - Identify and remove duplicate rows based on unique identifiers or key columns.
  - 
### 2. Removing Zero Variance Values
- **Description:** Eliminate features with zero variance, which do not contribute to analysis or modeling.
- **Actions:**
  - Identify columns with zero variance (i.e., constant values).
  - Remove these columns from the dataset.
  - 
### 3. Removing Unique Values
- **Description:** Remove features containing unique values, which do not provide meaningful insights.
- **Actions:**
  - Identify columns with unique values.
  - Remove these columns from the dataset.
  - 
### 4. Outlier Treatment using Boxplot IQR Method
- **Description:** Identify and handle outliers using the Interquartile Range (IQR) method with boxplot visualization.
- **Actions:**
  - Visualize distributions using boxplots.
  - Define the outlier threshold based on the IQR.
  - Replace or remove outliers based on the defined threshold.
  - 
### 5. Standardization Technique
- **Description:** Standardize numerical features to ensure consistency and comparability.
- **Actions:**
  - Scale numerical features to have a mean of 0 and a standard deviation of 1.
  - Apply standardization techniques such as Z-score normalization.
  - 
### 6. Capping and Flooring
- **Description:** Limit extreme values by capping (upper bound) and flooring (lower bound) numerical features.
- **Actions:**
  - Define upper and lower bounds based on domain knowledge or statistical methods.
  - Replace extreme values with the defined bounds.
  - 
### 7. Removing Highly Correlated Variables
- **Description:** Address multicollinearity by identifying and removing highly correlated variables.
- **Actions:**
  - Calculate correlation coefficients between variables.
  - Identify variables with high correlation (e.g., correlation coefficient > 0.7).
  - Remove one of the correlated variables to mitigate multicollinearity.
  - 
### 8. Addressing Multicollinearity with VIF > 5
- **Description:** Address multicollinearity by calculating Variance Inflation Factor (VIF) and removing variables with VIF greater than 5.
- **Actions:**
  - Calculate VIF for each variable in the dataset.
  - Identify variables with VIF greater than 5, indicating multicollinearity.
  - Remove one of the multicollinear variables to reduce multicollinearity.
  - 
## Conclusion
By following these specific data cleansing steps, we ensure that the dataset is cleansed of duplicates, irrelevant features, outliers, and multicollinear variables, resulting in high-quality data ready for analysis or modeling.
