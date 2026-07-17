Aggregate Functions analyze and summarize a set of values
These functions are "`min()`", "`max()`", "`count()`", "`mean()`", "`sum()`" etc. which can also be used by `groupby()` function to obtain data of a specific type of data

#### For whole Data Frame
```python
df.mean(numeric_only= True)
```
- same for all other aggregate functions, except count()
  for count() function -> `df.count()`

#### For single column
```python
df["ColumnName1"].sum()
```
- we are considering the column taken has numerical values only

#### Use with groupby() function
With `groupby()` function, a group of rows are selected and based on the data required, specific columns are summoned

Example-
```python
group=df.groupby("Column1")
group["Column2"].mean()
```
- again considering the "Column2" must have numerical values only

