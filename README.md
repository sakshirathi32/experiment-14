Aim:

To process a dataset and handle missing values efficiently.

Theory:

In data science, missing values are generally represented as NaN (Not a Number). Handling these missing values is an essential part of data preprocessing because incomplete data can affect analysis, lower model accuracy, and sometimes cause errors in algorithms. Missing values are usually managed by replacing them with statistical values such as Mean (average), Median (middle value), or a fixed constant like 0. Data cleaning also involves correcting inconsistencies such as different date formats or variations in text formatting like “cse” and “CSE” to maintain data consistency and accuracy.

isna()
This function returns a Boolean DataFrame where missing values are marked as True and available values are marked as False.

notna()
This is the opposite of isna(). It returns True for valid values and False for missing values.

sum()
When used with isna(), it counts the total number of missing values in each column.

sum(axis=1)
This calculates how many missing values are present in each row of the dataset.

dropna()
This function removes rows or columns that contain missing values, helping in cleaning incomplete data.

fillna(value)
This is used to replace missing values with a specified value such as a constant number, mean, or median.

replace(old, new)
This function searches for unwanted symbols or placeholder values like “-” and replaces them with proper NaN values for easier processing.

to_numeric()
This converts column values into numeric form. If invalid values are found, using errors='coerce' converts them into NaN.

mean()
This calculates the average value of a numerical column and is commonly used for filling missing data.

median()
This finds the middle value of a dataset and is especially useful when the data contains outliers.

str.upper()
This converts all text values in a column into uppercase letters, ensuring uniformity in categorical data.

pd.to_datetime()
This function changes different date formats into one standard date-time format, making the data more consistent.

Conclusion:

This program explains that data wrangling is a step-by-step process used to prepare raw data for analysis. By replacing incorrect placeholders with NaN, filling missing values using Mean or Median, and standardizing text and date formats, the dataset becomes clean, organized, and ready for reliable analysis. This improves the overall quality of data and supports accurate decision-making.
