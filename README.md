# EXPERIMENT - 14

AIM - Data Binning and Data Formatting using Python

THEORY: Data Binning and Data Formatting using Python
Data preprocessing is an essential step in data analysis, where raw data is transformed into a clean and meaningful format.
In this experiment, we use the libraries Pandas and NumPy to perform data binning and data formatting operations.

1. Importing Libraries

import pandas as pd

Imports the Pandas library.

pd is an alias used to call Pandas functions easily.

Used for handling tables (DataFrames).

import numpy as np

Imports NumPy library.

Used for numerical operations and arrays.

3. Creating Data

np.random.seed(0)

Sets a fixed seed value.

Ensures the same random numbers are generated every time you run the program.

pd.DataFrame({...})

Creates a DataFrame (table).

Data is given in dictionary format (column name → values).

Example:

'Price': np.random.randint(100, 1000, 10)

Generates 10 random integers between 100 and 1000.

5. Displaying Data

print(df)

Prints the complete dataset.

7. Data Binning
   
pd.cut(column, bins, labels=...)

Used to divide continuous data into categories (bins).

Example:

df['Price_Category'] = pd.cut(df['Price'],
                             bins=[0, 300, 700, 1000],
                             labels=['Low', 'Medium', 'High'])
Explanation:

bins: Defines range intervals

labels: Names given to each interval

Creates a new column with categories

9. Checking Data Types
   
df.dtypes

Displays the data type of each column (int, float, object, etc.)

11. Type Conversion

df['Price'] = df['Price'].astype(float)

Converts data type of column to float.

13. String Operations

df['Category'].str.upper()

Converts all text values to uppercase.

Example:

electronics → ELECTRONICS

15. Rounding Values
    
df['Order_Value'].round(2)

Rounds values to 2 decimal places.

17. Sorting Data
    
df.sort_values(by='Price')

Sorts data in ascending order.

df.sort_values(by='Price', ascending=False)

Sorts data in descending order.

19. Unique Values

df['Category'].unique()

Returns all unique values in a column.

20. Adding New Columns
    
df['New_Column'] = ...

Creates a new column based on some logic.

Example:

df['Order_Value'] = df['Price'] * df['Units_Sold']

22. Head Function
    
df.head()

Displays first 5 rows of dataset.

24. Tail Function
    
df.tail()

Displays last 5 rows of dataset.

26. Describe Function
    
df.describe()

Gives statistical summary:

Mean

Min

Max

Standard deviation

28. Shape of Data
    
df.shape

Returns number of rows and columns.

Example: (10, 5)

30. Columns Name
    
df.columns

Lists all column names.

32. Indexing / Accessing Data
    
df['Price']

Accesses a specific column.

df.loc[0]

Accesses row by label (index).
