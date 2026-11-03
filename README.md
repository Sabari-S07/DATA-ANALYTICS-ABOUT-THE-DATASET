# DATA-ANALYTICS-ABOUT-THE-DATASET
# AIM
To perform data analytics on a given dataset using Python and Pandas, understand the characteristics of the dataset, identify different types of data, examine missing values, and prepare the dataset for further analysis and machine learning.
# THEORY
The Python ecosystem, specifically the Pandas library, provides high-performance, easy-to-use data structures and data analysis tools built on top of NumPy. This experiment executes five critical theoretical phases of data preprocessing:

1. Data Structure Ingestion

Pandas handles structured data through two primary objects:
• Series: A 1D labeled array capable of holding any data type (equivalent to a single column).
• DataFrame: A 2D labeled data structure with columns of potentially different types (equivalent to a SQL table or Excel sheet).
• Functions used: pd.read_csv() or pd.read_excel() load raw storage formats into active RAM.

2. Structural & Descriptive Auditing

Understanding the dataset's scale and footprint requires evaluating its dimensions and memory allocations:
• Shape: Dictates the sample size (rows) and feature space (columns).
• Information Schema: Maps out data types, non-null counts, and memory usage.
• Functions used: df.shape, df.info(), and df.describe() (for central tendency, dispersion, and quartiles).

3. Data Type Identification

Variables must be properly cast to ensure mathematical operations function correctly:
• Numerical: Continuous or discrete quantitative values (Pandas types: int64, float64).
• Categorical: Qualitative text labels or discrete groups (Pandas types: object, category).
• Temporal: Date and time markers requiring chronological sequencing (Pandas type: datetime64).
• Functions used: df.dtypes to inspect types, and df.astype() to reprogram incorrect allocations.

4. Missing Value Diagnostics

Missing records (represented as NaN or None in Python) occur due to collection errors or systemic omissions. They fall into three theoretical buckets:
• Missing Completely at Random (MCAR): The missingness has no relationship with any data values.
• Missing at Random (MAR): Missingness is systematic and depends on other observed variables.
• Missing Not at Random (MNAR): The missing value depends on the unobserved value itself.
• Functions used: df.isnull().sum() to count gaps, and df.isnull().mean() * 100 to find the missing percentage per column.

5. Data Imputation & Sanitization Strategy

Machine learning algorithms generally cannot process datasets containing missing values. To prepare the data, we apply remediation strategies:
• Dropping Data: Used only if missingness is negligible (<5%) or localized to an entire useless column.
• Statistical Imputation: Filling numeric gaps with the mean (for normal distributions) or median (to resist outliers).
• Mode Imputation: Filling categorical gaps with the most frequent value.
• Functions used: df.dropna(), df.fillna(), or df.drop_duplicates().
# RESULT
The given dataset was successfully loaded and analyzed using Python and Pandas. The structure of the dataset, number of rows and columns, column names, data types, missing values, and statistical characteristics were identified.

The analysis provided a better understanding of the dataset and helped identify the necessary preprocessing steps. The dataset can now be further cleaned, visualized, and prepared for advanced data analytics or machine learning applications.
