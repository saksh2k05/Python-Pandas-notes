Filtering means keeping the rows that match the given condition

- Create a new variable to set the condition and use the variable to summon the filtered rows
  Example-
```python
    greater_than_1000  = df[df["Column"] >/</=/== condition]
    print(greater_than_1000)
```
-  To filter rows using 2 or more conditions, using logical operators of C language(`&(and), | (or)` ) is preferred

  Example
  
``` python
 w= df[(df["Column1"]>=100) |
	        (df["Column2"]== "Yes")]
```
	result gives rows having Column1>=100 OR Column2=Yes
	
```python
f=df[(df["Column3"]>=100) &
	        (df["Column4"]== "Yes")]
```
	result gives rows having Column3>=100 AND Column4=Yes