JSON- JavaScript Object Notation
CSV- Comma Separated Values

To need to access a CSV or JSON file, we first need its location
We use "`read_csv()`" and "`read_json()`" to read these files

```python
df= pd.read_csv(r"Location of file")
```
- `df.to_string()` is used to print THE WHOLE ARRAY, else the displayed data is TRUNCATED

- To change the default indexing of data, use "index_col"
```python
df= pd.read_csv("Location of file", index_col="Name")
```
`df.to_csv(xyz.csv)` -> pushes a table to a **.csv** file


