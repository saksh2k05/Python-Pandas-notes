Process of removing or filtering out incomplete or irrelevant data

#### 1) Dropping irrelevant columns
`drop()` function will be used
```python
df= df.drop(columns=["Column1", "Column2"])
```

#### 2) Handle missing data
`dropna()` meaning 'drop not available available values' and `fillna()` meaning 'fill not available values' functions will be used
```python
df= df.dropna(subset=["Column4"])
df= df.fillna({"Column6": "num1", "Column3": "num5"})
```

#### 3) Fix inconsistency
```python
df["ColumnName5"] = df["ColumnName5"].replace({"Value1": "num4", "Value2": "num2"}) 
```

#### 4) Standardize text
```python
df["ColumnName"] = df["ColumnName"].str.lower()
```
`lower()` , `upper()`, `title()`, etc. can be used

#### 5) Fix Datatypes
```python
df["Column"]= df["Column"].astype(object)
```
any relevant data type can be used according to the requirement

#### 6) Remove Duplicate Values
It removes all the duplicate rows
```python
df= df.drop_duplicates()
```
     use keep='first' and inplace=True for keeping the first element and delete the rest of the elements


     Example
```python
     df.drop_duplicates(  
     subset=['column'],  
     inplace=True 
     )
```

