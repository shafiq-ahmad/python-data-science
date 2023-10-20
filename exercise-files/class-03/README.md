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

## Using sample data from seaborn

### Import data

```python
df_tips = sns.load_dataset('tips')
df_tips.head()
```

### Export data to CSV

```python
df_tips.to_csv('./data/tips.csv')
```

## Reverse order

```python
df_tips.loc[::-1] 
```

reverce order with new indexes

```python
df_tips.loc[::-1].reset_index(drop=True).head()
```

## Select column by datatype

```python
df.select_dtypes(include=['number']).head() # select only cols having number types
df.select_dtypes(exclude=['number']).head() # select only cols not having number types
```

### Reduce dataframe size

```python
df_tips.sample(frac=0.1).shape   #get 10%
```

### Copy data from clipboard

```python
df_ship = sns.load_dataset('titanic')
df_ship.to_excel('ship.xlsx')
# First copy some data from above file
df_ship = pd.read_clipboard()
```

- Split and join data in 2 dataframes
- Agregate by mulitple groups/function
- Selecting rows/colums
- Reshaping multiindex series
- Continues to categorical data conversion: Creating bins
- Convert one set of value to another
- Transpose a wide dataframe
- Reshaping a dataframe
