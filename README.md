# Formative Assessment Data Preprocessing

## **SCOPE**
The main objective of this project is to design and implement a robust data preprocessing system that addresses common challenges such as missing values, outliers, inconsistent formatting, and noise. By performing effective data preprocessing, the project aims to enhance the quality, reliability, and usefulness of the data for machine learning.

## **Data Exploration:**
The scope of this Data Exploration for the dataset "Employee.csv" is to generate a comprehensive report detailing the basic information about the data for to understand the unique values and feature of it and to Perform the statistical analysis in the renaming numerical columns. By using,
Info
Head and Tail
Shape
Null and Duplicate values
Describe, etc.
Additionally, the analysis includes checking and finding outliers in the "Age" and "Salary" column by plotting a box plot and IQR method.

## **Data Cleaning:**
- 1. Load the Data: First, import the necessary libraries (Pandas and Numpy) and load your dataset using the "pd.read_csv" function.
- 2. Treat Inappropriate Values: Identify and treat any inappropriate values in your dataset. i.e., values in the "Gender" column are numerical values, and they are converted to male and female, respectively.
- 3. Remove Duplicate Rows: Use the Pandas drop_duplicates function to remove any duplicate rows from your dataset. This ensures that each row in your dataset is unique.
- 4. Find and Treat Outliers: Identify outliers using the Interquartile Range (IQR) method. Calculate the first quartile (Q1) and third quartile (Q3) for each numerical column, and then determine the IQR. Outliers are typically values below Q1 (1.5 * IQR) or above Q3 (1.5 * IQR). Replace these outliers with NaN.
- 5. Replace Zero and Nan Values in Age and Salary : Specifically for the Age and Salary  column, replace any zero and Nan values with Mean vale becose the is no any outliers in the dataset.
- 6. Treat Null Values: Handle missing values in all columns appropriately. For categorical columns, fill in the in the missing values with the mode value.

## **Key Findings:**
Using box plot analysis, it can conclude that the IQR (Interquartile Range) method is the best way to remove outliers.
