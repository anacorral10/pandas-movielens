
# Case Study: Movie Data Analysis
This Jupyter notebook contains a case study I used to learn pandas, the primary data analysis library in Python.
This case study uses a dataset from the IMDB [MovieLens website](https://grouplens.org/datasets/movielens/).

Using the IMDB based movielens data set, I analyzed the average movie ratings over time to answer the following questions:

* Are Movie ratings related to the year of launch?
* Do some years look better for the boxoffice movies than others?
* Does any data point seem like an outlier in some sense?

## How I used Pandas to Analyze the Dataset:

In this notebook, I analyzed three CSV files:
* **ratings.csv** : userId, movieId, rating, timestamp
* **tags.csv** : userId, movieId, tag, timestamp
* **movies.cs** : movieId, title, genres

### Data Ingestion:
* Using the `read_csv` function in pandas, I ingested the three CSV files
* Converted the CSV files to Pandas *Dataframes* and *Series*

### Statistical Analysis
* Performed basic statistical operations on the Series and DataFrames
* Used Descriptive Statistics to look at how the ratings are distributed
* Used individual functions for generating `min()`, `max()`, and standard deviation `std()` values, mode of data `mode()`, as well as functions for correlation analysis `corr()`

### Data Cleaning
* Performed data preparation and exploration (detection) options in Pandas like `isnull()`, `any()`, and `dropna()` functions.

### Data Visualization
* Performed inline plotting
* Created *box plots*, and *histograms* using Pandas's `plot()` function.
* Adjusted the access formatting and other window properties by changing the limits on the Y-axis

### Data Transformation
* Performed slicing of some columns
* Filtered data frame rows
* Aggregated data using the `groupby()` operation
  * Then, executed basic statistical functions on these groups using `mean()` and `count()` operations

### Merging Dataframes
* Joined data from multiple data frames using inner joins and other operations such as: `merge()`, `how = inner`, `on = keys`

### String Operations
* Performed three main string operations: `split()`, `contains()`, and `extract()`

### Timestamps
* Learned how to work with timestamps using:  POSIX Time, `to_dateTime()`
* Used Data type `datetime64[ns]`
* Selected rows based on timestamps
* Sorted tables in chronological order

## To Download the Dataset:
Please note that if you would like to analyze this dataset you will need to download it. The folder was too large to fit on this platform due to size constraints.

Here are the links to the data source and location:
* *Data Source:* MovieLens web site (filename: ml-25m.zip)
* *Location:* https://grouplens.org/datasets/movielens/

It should be the first zip file on the page
Once the download completes, please make sure the data files are in the directory of the jupyter notebook folder.


## More information about Pandas:
**Pandas** is a Python library for data analysis. It offers a number of data exploration, cleaning and transformation operations that are critical in working with data in Python.

pandas build upon numpy and scipy providing easy-to-use data structures and data manipulation functions with integrated indexing.

The main data structures pandas provides are Series and DataFrames. After a brief introduction to these two data structures and data ingestion, the key features of pandas this notebook covers are:

* Generating descriptive statistics on data
* Data cleaning using built in pandas functions
* Frequent data operations for subsetting, filtering, insertion, deletion and aggregation of data
* Merging multiple datasets using dataframes
* Working with timestamps and time-series data


**Additional Resources:**

pandas Documentation: http://pandas.pydata.org/pandas-docs/stable/

Python for Data Analysis by Wes McKinney

Python Data Science Handbook by Jake VanderPlas

