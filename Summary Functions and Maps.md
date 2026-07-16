
### `describe()`

  `describe()` is a function that gives a *complete summary* of the dataframe provided, including mean, count, max etc.
  
```python 
df.Column1.describe() 
```
is used to describe properties of a single column

- Functions like `mean()`, `values_counts()` , `unique()`, etc are used along with the name of column of the given DataFrame to obtain the desired values
  Example- 
  ```python
  df.Column4.mean() #to calculate mean
  df.Column2.value_counts() #to count the values
  df.Column1.unique() #to find out all the unique values
  ```

