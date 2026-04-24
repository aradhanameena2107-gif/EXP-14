# EXPERIMENT 14

AIM:

To study and implement data binning and data formatting using Python (Pandas library) by creating datasets and applying functions like pd.cut(), value_counts(), unique(), round(), str.upper(), sort_values(), and dtypes for organizing, categorizing, and analyzing data effectively. This helps in converting raw data into meaningful and structured information.

THEORY:

1. Data Binning

Data binning is a technique used to convert continuous numerical data into discrete groups or categories (bins). It reduces complexity, removes noise, and makes data easier to analyze and interpret, especially when dealing with large datasets.

Functions Used:

a) pd.cut()

Used to divide numerical data into intervals (bins).
Converts continuous values into categorical labels.
Makes comparison and analysis easier.

Applications in experiment:

Price → Low, Medium, High (helps classify product cost levels)
Units_Sold → Low Sales, Medium Sales, High Sales (helps analyze demand)
Order_Value → Low, Medium, High (helps categorize transaction size)
Delivery_Time → On Time, Delayed, Critical (helps evaluate service efficiency)

b) value_counts()

Counts the number of values in each category.
Helps in understanding frequency distribution of data.
Useful for identifying which category has the highest or lowest data.

c) unique()

Returns all distinct values from a column.
Helps to verify whether binning or categorization is done correctly.

2. Data Formatting

Data formatting ensures that the dataset is clean, consistent, and easy to read, which is important before performing analysis.

Functions Used:

a) df.dtypes

Displays the data type of each column (int, float, object, etc.).
Helps in identifying incorrect data types and ensures proper processing.

b) round()

Rounds numerical values to a specified number of decimal places.
Improves readability and avoids unnecessary precision.
Example use:
Price values rounded to make them simpler and uniform.

c) str.upper()

Converts all text data into uppercase.
Ensures uniformity and avoids case-sensitive issues during analysis.

d) astype()

Used to change the data type of a column.
Important when performing calculations or formatting data properly.


3. Data Sorting

Function:
 sort_values()
Used to arrange data in a specific order (ascending or descending).
Helps in identifying trends such as highest or lowest values.

Types:

Ascending (default) → lowest to highest
Descending → highest to lowest (ascending=False)


4. DataFrame Creation
   
Function: pd.DataFrame()
Used to create structured tabular data from dictionaries or lists.
Forms the base for performing all operations.

Datasets used:

Product dataset (Price, Units Sold, etc.)
Order dataset (Order Value, Delivery Time, etc.)


5. Libraries Used
   
Pandas (pd) → Used for data manipulation, binning, formatting, and analysis
NumPy (np) → Used for numerical operations (supporting library)


CONCLUSION:

The experiment successfully demonstrates how data binning and formatting techniques are used in data preprocessing. By using pd.cut(), continuous data is converted into meaningful categories, making it easier to analyze patterns and trends.

Functions like value_counts() and unique() help in understanding and verifying the data distribution. Formatting functions such as round() and str.upper() improve consistency and readability, while sort_values() helps in organizing the data systematically.

Thus, this experiment highlights the importance of data cleaning, transformation, and organization, which are essential steps in data analysis, helping in better decision-making and accurate interpretation of data.
