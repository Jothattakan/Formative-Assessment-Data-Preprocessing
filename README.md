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
-  Load the Data: First, import the necessary libraries (Pandas and Numpy) and load your dataset using the "pd.read_csv" function.
-  Treat Inappropriate Values: Identify and treat any inappropriate values in your dataset. i.e., values in the "Gender" column are numerical values, and they are converted to male and female, respectively.
-  Remove Duplicate Rows: Use the Pandas drop_duplicates function to remove any duplicate rows from your dataset. This ensures that each row in your dataset is unique.
-  Find and Treat Outliers: Identify outliers using the Interquartile Range (IQR) method. Calculate the first quartile (Q1) and third quartile (Q3) for each numerical column, and then determine the IQR. Outliers are typically values below Q1 (1.5 * IQR) or above Q3 (1.5 * IQR). Replace these outliers with NaN.
-  Replace Zero and Nan Values in Age and Salary : Specifically for the Age and Salary  column, replace any zero and Nan values with Mean vale becose the is no any outliers in the dataset.
-  Treat Null Values: Handle missing values in all columns appropriately. For categorical columns, fill in the in the missing values with the mode value.

## **Data Analysis: :**
- Filtered the data with age >40 and salary<5000.
- Plotting the scatter plot chart with age and salary.
- Plotting bar chart to visualize the number of people from each place.

## **Data Encoding:**
Convert categorical variables in the columns "Company", "Place", "Country" and "Gender" into numerical representations using techniques such as one-hot encoding to make them suitable for analysis by machine learning algorithms.

## **Feature Scaling:**
After encoding, feature scaling of numerical columns is performed using the standardscaler and minmaxscaler.

## **Key Findings:**
- There are 148 rows and 6 columns in the dataset.
- Out of 6 columns, 3 are categorical and 3 are numerical columns. But one of the numerical columns is the label encoding the employee's gender.
- There are 6 companies located in 11 places in India present in the dataset.
- There are four duplicate values present in the dataset.
- The missing values in the column Company and Place can be replaced with the mode value; the missing values in the column Age and Salary can be replaced with the mean value; and the values in the column gender are in appropriate can be replaced with Male and Female accordingly.
