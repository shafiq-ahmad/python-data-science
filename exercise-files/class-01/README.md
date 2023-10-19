
# Class 01: Introduction

## Jupitor notebook

Used for data visualization and data science
You can use markdown language (.md file) within for making notes or documentation.
Code consists of cells and code within the cell can be run seperately and results appear below the cell.

**File extension:** .ipynb

## Important libraries and their usage

- pandas: A powerful data manipulation and analysis library for handling structured data, with extensive functionality for reading, writing, and transforming data, often used for Excel-like functionality in data processing.
- numpy: A fundamental library for numerical computing in Python, providing support for large, multi-dimensional arrays and matrices, as well as a collection of mathematical functions to operate on these arrays.
- matplotlib: A data visualization library that creates static, animated, or interactive plots and graphs, widely used for data visualization and presentation.
- seaborn: An extension of matplotlib, seaborn provides a high-level interface for creating aesthetically pleasing and informative statistical graphics, adding additional features and customization options to enhance data visualization.
- plotly: A versatile library for creating interactive and web-based data visualizations, offering a variety of charts, graphs, and dashboards that can be used for data exploration and presentation
- scipystats: This is not a specific library but might refer to the statistical modules available in SciPy. SciPy is an ecosystem of libraries built on NumPy, and it includes a subpackage for statistical functions and tests, providing various statistical tools and methods for data analysis.
- scikit-learn: A machine learning library that offers tools for data mining and data analysis, including various algorithms for classification, regression, clustering, and more, as well as utilities for preprocessing and model evaluation.
- streamlit: A framework for creating interactive web applications for data science and machine learning, allowing users to easily turn data scripts into shareable web apps and dashboards with minimal coding effort.

## Installing a library

Mehtod 1: go to cmd.exe. and you need to run 'pip install' followed by the library name.

> pip install pandas
>
>pip install numpy
>
> pip install matplotlib
>
> pip install seaborn

Mehtod 2: Inside VS Code Shell run the above commands

Mehtod 3: write above command in the cell of python file.

> pip install pandas numpy matplotlib seaborn plotly

### Importing libraries in the code

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import plotly as px
import seaborn as sns
```

### DataFrme

DataFrame is a 2-dimensional labeled data structure with columns of potentially different types. You can think of it like a spreadsheet or SQL table, or a dict of Series objects.

### Collecting Data

Primary data: also called orignal data, it is the data that is produces by you

Secondary data: that is produces by someone
Following are some sources of secondary data.

- kaggle.com
- google datasearch
- github
- faostats.com
- all website data scrap
- country stats website: like pakistan beuru of statistics
- crime detection DNA
- Nadra
- Business (stock exchange, price, etc)
- University data
- Research database
