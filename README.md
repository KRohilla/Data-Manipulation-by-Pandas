# Data-Manipulation-by-Pandas
<br>
Task 2 from Main Flow Services and Technologies
<br><br>
Pandas is a powerful and versatile Python library designed for data manipulation and analysis. 
It provides two main data structures: Series (1-dimensional) and DataFrame (2-dimensional). 
Below are some key techniques and methods used for data manipulation with Pandas:
<br>
<br>
<b> 1. Loading Data</b><br>
Reading Data:
pd.read_csv(), pd.read_excel(), pd.read_json(), and pd.read_sql() are commonly used to load data into a DataFrame. <br>
Writing Data:
df.to_csv(), df.to_excel(), df.to_json(), and df.to_sql() are used to export data from a DataFrame.
<br>
<br>
<b> 2. Data Selection and Filtering</b>
Viewing Data:
df.head(), df.tail(), df.info(), and df.describe() give you a quick overview of the data. <br>
Selecting Data:
Selecting columns: df['column_name'] or df[['col1', 'col2']]. <br>
Selecting rows: df.loc[] (label-based) or df.iloc[] (index-based). <br>

<b> 3. Filtering and Sorting</b> <br>
Filtering Rows:
Conditional filtering: df[df['column'] > value].<br>
Filtering with multiple conditions: df[(df['col1'] > value1) & (df['col2'] < value2)].<br>
Sorting:
Sorting by column: df.sort_values('column', ascending=False).<br>

<b> 4. Data Cleaning</b><br>
Handling Missing Data:
df.isnull() to detect missing values.<br>
df.dropna() to remove rows/columns with missing values.<br>
df.fillna(value) to fill missing values with a specific value.<br>
Removing Duplicates:
df.drop_duplicates() to remove duplicate rows.<br>
Renaming Columns:
df.rename(columns={'old_name': 'new_name'}).<br>

<b> 5. Data Transformation</b><br>
Applying Functions:
df.apply() to apply functions to DataFrame rows/columns.<br>
df['column'].map() for element-wise operations on a Series.<br>
Creating/Modifying Columns:
df['new_column'] = df['col1'] + df['col2'] to create or modify columns.<br>
Changing Data Types:
df['column'] = df['column'].astype('data_type') to change the data type of a column.<br>

There are so many other methods also, here we use some of the methods which we required during the filtering and cleaning our data. After these steps, we can also did exloratory data analysis, transformation of the data, data visualisation and advanced operations on the data.
