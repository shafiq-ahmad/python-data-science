# Class 02: Importing data from excel

## Step 1

```python
# import libraries
import pandas as pd

```

## Step 2

```python
# import data
df = pd.read_excel("./data/sample-data.xlsx")
```

## Step 3

```python
# Show summary of DataFrame
df.describe()
```

## Step 4

```python
# Listing all columns
df.columns
```

## Step 5

```python
# By index
df.sort_index()

# Sort by value (a column)
df.sort_values(by = "weight")
```

## Type casting of a column

```python
# Cast the `height` column to the `int` data type
df['height'] = df['height'].astype('int')

# Print the DataFrame
print(df)
```
