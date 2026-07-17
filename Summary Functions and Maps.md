
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

### Maps

Used to transform existing data into a new representation or format

`map()` works on a Series, applies a function to each value and returns a new Series

```python
review_points_mean = reviews.points.mean()
reviews.points.map(lambda p: p - review_points_mean)
```


`apply()` works on a DataFrame, applies a custom function to each row or column

```python
def remean_points(row):
row.points = row.points - review_points_mean
return row

reviews.apply(remean_points, axis='columns')  # row-wise
reviews.apply(remean_points, axis='index')    # column-wise
```

Key point: both `map()` and `apply()` return a new Series or DataFrame respectively, they do not modify the original data
