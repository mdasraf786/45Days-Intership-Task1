🧹 Data Cleaning Process(In Excel)

The dataset contained customer demographic, spending, and campaign response details. To prepare it for analysis, the following cleaning steps were applied:

Removed Irrelevant Columns

Dropped ID column since it does not contribute to analysis.

Handled Missing Values

Found ~20–30 rows with missing values in Income → removed those rows.

Checked for Duplicates

Verified dataset for duplicate rows → none found.

Feature Engineering & Fixes

Age = Current Year – Year_Birth.

TotalSpending = sum of all product-related spending columns.

TotalAcceptedCmp = sum of campaign acceptance columns.

Converted Dt_Customer to proper Date format.

Categorical Variable Standardization

Education (renamed → UpdatedEducation):

Basic, 2n Cycle → Secondary

Graduation → Graduate

Master, PhD → Postgraduate

Marital_Status (renamed → UpdatedMarital_Status):

Married, Together → Married

Single, Alone, Widow, Divorced → Single

Absurd, YOLO → Other

Outlier Treatment

Year_Birth → removed unrealistic ages (below 18 or above 100).

Income → removed extreme outliers using IQR method.

Final Dataset Columns

Year_BirthWithoutOutliers, UpdatedEducation, UpdatedMarital_Status,
IncomeWithoutOutliers, Kidhome, Teenhome, Age, Dt_Customer, Recency,
TotalSpending, NumDealsPurchases, NumWebPurchases, NumCatalogPurchases,
NumStorePurchases, NumWebVisitsMonth, TotalAcceptedCmp, Complain, Response

✅ The dataset is now consistent, free of missing values, duplicates, and outliers, with standardized categories and properly formatted features.
It is ready for Exploratory Data Analysis (EDA) and modeling.


✅ The dataset is now consistent, free of missing values, duplicates, and outliers, with standardized categories and properly formatted features. It is ready for Exploratory Data Analysis (EDA) and modeling.
