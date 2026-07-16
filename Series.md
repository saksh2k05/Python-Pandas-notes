
Series -> 1D array

`series= pd.Series(data, index=["a", "b", "c"])`

- index section defines how I would like to represent my data

- dtype states the data type of the given series(strings are shown as "objects" under dtype)

- `series.loc["c"]  
  "loc" is used to find the data using the index and also manipulating the data
  Examples:
```python
  `series.loc["c"]= 200
```
```python
  `series.loc["a"]+=43
```

- `series.iloc[0]
  "`iloc`" is used to find a value using the original index value of the element
  series.iloc[0] -> gives the value of the 0th index value of given data

- `series[series condition]
  under [condition], comparative operators are used to filter by values
  ex- `series[series>200]` gives all values in data that are greater than 200

- `series.astype(datatype)

  astype is used to display the data in a different format from the current one
  Ex- `series.astype(str)`
```python
  series=pd.Series(dtype=datatype)` 
```
   can also be used to vary data type
  
- [ ...] operator is used to depict a series
