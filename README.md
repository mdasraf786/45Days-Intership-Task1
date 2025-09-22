🧹 Data Cleaning Process(In Excel)

The dataset contained customer demographic, spending, and campaign response details. To prepare it for analysis, the following cleaning steps were applied:

Removed Irrelevant Columns

Dropped ID column since it does not contribute to analysis.

Handled Missing Values

Found ~20–30 rows with missing values in Income → removed those rows.

Created / Fixed Features

Added Age column = Current Year – Year_Birth.

Converted Dt_Customer to proper Date format.

Created TotalSpending = sum of all product-related spending columns.

Categorical Variable Standardization

Education: grouped into Secondary (Basic, 2n Cycle), Graduate (Graduation), and Postgraduate (Master, PhD).

Marital_Status: simplified into Married, Single, and Other categories.

Outlier Treatment

Year_Birth: removed unrealistic ages (below 18 or above 100).

Income: detected extreme outliers using IQR method and removed them.

Final Dataset Columns

Year_BirthWithoutOutliers, UpdatedEducation, UpdatedMarital_Status,
IncomeWithoutOutliers, Kidhome, Teenhome, Age, Dt_Customer, Recency,
TotalSpending, NumDealsPurchases, NumWebPurchases, NumCatalogPurchases,
NumStorePurchases, NumWebVisitsMonth, TotalAcceptedCmp, Complain, Response

✅ The dataset is now consistent, free of missing values, standardized, and ready for Exploratory Data Analysis (EDA) and modeling.
