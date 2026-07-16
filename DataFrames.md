
DataFrames -> 2D array

```python
df= pd.DataFrame(data, index=["a", "b", "c"])
```

Example- 

|     | Column1 | Column2 |
| --- | ------- | ------- |
| a   | name1   | value1  |
| b   | name2   | value2  |
| c   | name3   | value3  |


- indexing, loc and iloc, conditional outputs are same as Series

- Add a new column
```python
  df["Column3"]= ["num1", "num2", num3"]
```
  
  Example-

|     | Column1 | Column2 | Column3 |
| --- | ------- | ------- | ------- |
| a   | name1   | value1  | num1    |
| b   | name2   | value2  | num2    |
| c   | name3   | value3  | num3    |

- Add a new row
  A new row is to be defined for the respective data frame, and then to be concatenated with the original dataframe
  
```python
  new_row = pd.DataFrame([{"Column1": "name4", "Column2": "value4", "Column3": "num4"}], index=["d"])
  df = pd.concat([df, new_row])
```
  >Example

|     | Column1 | Column2 | Column3 |
| --- | ------- | ------- | ------- |
| a   | name1   | value1  | num1    |
| b   | name2   | value2  | num2    |
| c   | name3   | value3  | num3    |
| d   | name4   | value4  | num4    |

- To rename columns
```python
  df = df.rename(columns={"OldName1": "NewName1", "OldName2": "NewName2"})
```

- Here are a few useful functions
    
    `df.head(n)`       -> first n rows (default 5) 
    `df.tail(n) `     -> last n rows 
    `df.shape`           -> (no. of rows, columns) 
    `df.info()`         -> column names, dtypes, non-null counts 
    `df.describe()` -> statistical summary of numerical columns 
    `df.columns`       -> list of column names 
    `df.dtypes`         -> datatype of each column

 -  [[ ...] ] operator is used to depict a Data Frame
   
 - The `set_index()` method can be used to set a column as the index column, and it's values to be index values
   Ex- 
```python
   df.set_index("ColumnA")
```

