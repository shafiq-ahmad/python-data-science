# Pandas Tips and Tricks

## Import libraries

```python
import pandas as pd
import numpy as np
import seaborn as sns
```

## Get Pandas version

Method 1

```python
pd.__version__     #only version
```

Method 2

```python
pd.show_versions() #show all details
```

## Creating Data Frame

### Method 1

```python
# assigning dictionary
df = pd.DataFrame({'A col': [1,2,3], 'B col':[3,4,5]})
print(df)
```

```python
# Assigning NumPy array
arr = np.array([[1,2,3],[4,5,6],[7,8,9]])
df = pd.DataFrame(arr)
print(df)
```

```python
# Using random number
df = pd.DataFrame(np.random.rand(4,8), columns=list('ABCDEFGH'))
print(df)
```

### Renaming a column

Method 1: using rename() method

```python
df.rename(columns={'A':'A_col'}, inplace=True)
df
```

Method 2: assign a new list of column names

```python
df.columns=['B','col_bb','C','D','E','F','G','H']
df
```
