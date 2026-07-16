-  Selection by Column
```python
  df["Column1", "Column2", "Column3"].to_string()
```
- Selection by Row

```python
  df.loc["Value Of Row"]
```

    In order to display only the selected columns with the desired rows, mention the column names along with the rows selection- 
     df.loc["Row2" : "Row6" , ["Column1", "Column2"]]
    
    To locate using iloc, 
```python
df.iloc[starting row : ending row : steps, starting column : ending column]
```
    - *ending value will not be inclusive
    - n steps will display every nth row*

- 
```python
df.loc[ : , ['Column1' , 'Column2', 'Column3', ...]]'''
```
   is used to select all rows belonging to the specific columns only
   
- `isin` is lets you select data whose value "is in" a list of values
  `df.loc[df.column.isin(['Row_value1', 'Row_value2'])]