---
layout: page
title: Pandas Reference
description: >-
    Python Reference Guide
nav_order: 4
---

# Pandas Reference

{:.no_toc}
Created by Brandon Concepcion
{: .no_toc .text-delta }

## Table of Contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## What is Pandas?
[Pandas](https://pandas.pydata.org/docs/index.html){:target="_blank"} is a powerful data manipulation and analysis library in Python. It provides two main data structures:

* `DataFrame`: A 2-dimensional tabular data structure with labeled axes (rows and columns), similar to a spreadsheet in Excel or Google Sheets
* `Series`: A 1-dimensional labeled array capable of holding any data type. You can think of these as the columns of a DataFrame


## Pandas
In the examples in the left column, `pd` refers to the Pandas library. `df` refers to a generic DataFrame.

| **Name**                         | **Description**                                                                                         | **Input**                                         | **Output**                                  |
|----------------------------------|---------------------------------------------------------------------------------------------------------|--------------------------------------------------|---------------------------------------------|
| `pd.read_csv()`                  | Reads a CSV file into a DataFrame.                                                                       | **string**: filename                             | **DataFrame**: contents of the CSV file     |
| `df.head(n)`                     | Displays the first `n` rows of the DataFrame. Defaults to 5 if `n` is not provided.                      | (Optional) **int**: number of rows to display    | **DataFrame**: first `n` rows               |
| `df.tail(n)`                     | Displays the last `n` rows of the DataFrame. Defaults to 5 if `n` is not provided.                       | (Optional) **int**: number of rows to display    | **DataFrame**: last `n` rows                |
| `df.info()`                      | Provides a summary of the DataFrame, including column data types and non-null values.                    | None                                             | **Summary**: information about DataFrame    |
| `df.describe()`                  | Generates descriptive statistics like mean, min, max for numerical columns.                             | None                                             | **DataFrame**: summary statistics           |
| `df.shape`                       | Returns the number of rows and columns in the DataFrame.                                                 | None                                             | **tuple**: (rows, columns)                  |
| `df.columns`                     | Lists the column names in the DataFrame.                                                                 | None                                             | **Index**: column names                     |
| `df.dtypes`                      | Shows the data types of each column in the DataFrame.                                                    | None                                             | **Series**: data types of each column       |
| `df.isnull()`                    | Returns a DataFrame showing Boolean values for missing data.                                             | None                                             | **DataFrame**: True/False for null values   |
| `df.dropna()`                    | Removes rows with missing values.                                                                        | None                                             | **DataFrame**: without missing rows         |
| `df.fillna(value)`               | Fills missing values with a specified value.                                                             | **value**: what to fill in for missing values    | **DataFrame**: missing values replaced      |
| `df.sort_values(by)`             | Sorts the DataFrame by the values in a column or multiple columns.                                       | **string**: column name <br> (Optional) `ascending=True/False` | **DataFrame**: sorted DataFrame |
| `df.groupby(by)`                 | Groups the DataFrame by one or more columns and allows aggregation.                                      | **string**: column name(s) to group by           | **DataFrameGroupBy**: object for aggregation|
| `df.drop(labels)`                | Drops specified rows or columns from the DataFrame.                                                      | **string**: column name or **list** of labels    | **DataFrame**: with columns/rows dropped    |
| `df.iloc[]`                      | Selects data by integer-location based indexing (row and column positions).                              | **int**: row/column index                        | **DataFrame/Series**: selected data         |
| `df.loc[]`                       | Selects data by label-based indexing (row/column names).                                                 | **string**: label or list of labels              | **DataFrame/Series**: selected data         |
| `df.rename(columns={'old':'new'})`| Renames columns or index of the DataFrame.                                                               | **dict**: old and new names for columns          | **DataFrame**: renamed columns              |
| `df.apply(function)`             | Applies a function to each element in a column or across a row/column.                                   | **function**: the function to apply              | **Series** or **DataFrame**: with results   |
| `df.merge(df2, on=key)`          | Merges two DataFrames based on a common column (key).                                                    | **DataFrame**: another DataFrame <br> **string**: key column | **DataFrame**: merged DataFrame          |
| `pd.concat([df1, df2])`          | Concatenates two or more DataFrames along a particular axis (rows or columns).                           | **list**: list of DataFrames                     | **DataFrame**: concatenated DataFrame       |


## GroupBy Aggregation Functions
These aggregation functions are most commonly applied after using the `.groupby()` method in Pandas, such as `df.groupby(agg_col).agg_func()`. Recall that the `.groupby()` method is used to perform group-wise operations. The `groupby()` method groups the data based on one or more columns, and then applies the aggregation functions to each one of the groups to compute the desired statistics.


| **Name**           | **Description**                                                            | **Output**                     |
|--------------------|----------------------------------------------------------------------------|-----------------------|--------------------------------|
| `mean()`           | Calculates the mean (average) of values in a column or group.               | **float**: mean of values      |
| `sum()`            | Sums all the values in a column or group.                                   | **float/int**: sum of values   |
| `min()`            | Returns the minimum value in a column or group.                             | **float/int**: minimum value   |
| `max()`            | Returns the maximum value in a column or group.                             | **float/int**: maximum value   |
| `count()`          | Counts the number of non-null entries in a column or group.                 | **int**: count of non-null rows|
| `median()`         | Calculates the median of values in a column or group.                       |  **float/int**: median value    |
| `std()`            | Calculates the standard deviation of values in a column or group.           | **float**: standard deviation  |
| `agg(func)`        | Applies a custom aggregation function (one the user would define) to a group.| **Series**: result of aggregation|
| `nunique()`        | Counts the number of unique values in a column or group.                    | **int**: count of unique values|
| `first()`          | Returns the first value in each group.                                      | **Series**: first values       |
| `last()`           | Returns the last value in each group.                                       |  **Series**: last values        |
| `mode()`           | Returns the mode (most frequent value) in a column or group.                |  **Series**: mode value         |
| `prod()`           | Returns the product of values in a column or group.                         |  **float/int**: product of values|
