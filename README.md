# Pandas- 🐼🐼

<img width="853" height="367" alt="image" src="https://github.com/user-attachments/assets/2f6c4b86-ea5b-44d5-874a-e935772e2ca7" />


-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Pandas is a core library for data science and data analysis in Python, providing intuitive and flexible data structures, such as the DataFrame. It simplifies the process of data cleaning, manipulation, and analysis, making it an essential tool for anyone working with data.

History
Developer Wes McKinney began working on Pandas in 2008 while at AQR Capital Management, driven by the need for a high-performance, flexible tool to perform quantitative analysis on financial data. Before leaving AQR, he was able to convince management to allow him to open-source the library.

Another AQR employee, Chang She, joined the effort in 2012 as the second major contributor to the library.

In 2015, Pandas signed on as a fiscally sponsored project of NumFOCUS, a 501(c)(3) nonprofit charity in the United States.

Data model
Pandas is built around data structures called Series and DataFrames. Data for these collections can be imported from various file formats such as comma-separated values, JSON, Parquet, SQL database tables or queries, and Microsoft Excel.[8]

A Series is a 1-dimensional data structure built on top of NumPy's array.[9]: 97  Unlike in NumPy, each data point has an associated label. The collection of these labels is called an index.[4]: 112  Series can be used arithmetically, as in the statement series_3 = series_1 + series_2: this will align data points with corresponding index values in series_1 and series_2, then add them together to produce new values in series_3.[4]: 114  A DataFrame is a 2-dimensional data structure of rows and columns, similar to a spreadsheet, and analogous to a Python dictionary mapping column names (keys) to Series (values), with each Series sharing an index.[4]: 115  DataFrames can be concatenated together or "merged" on columns or indices in a manner similar to joins in SQL.[4]: 177–182  Pandas implements a subset of relational algebra, and supports one-to-one, many-to-one, and many-to-many joins.[9]: 147–148 

Users can transform or summarize data by applying arbitrary functions.[4]: 132  Since Pandas is built on top of NumPy, all NumPy functions work on Series and DataFrames as well.[9]: 115  Pandas also includes built-in operations for arithmetic, string manipulation, and summary statistics such as mean, median, and standard deviation.[4]: 139, 211  These built-in functions are designed to handle missing data, usually represented by the floating-point value NaN.[4]: 142–143 

Subsets of data can be selected by column name, index, or Boolean expressions. For example, df[df['col1'] > 5] will return all rows in the DataFrame df for which the value of the column col1 exceeds 5.[4]: 126–128  Data can be grouped together by a column value, as in df['col1'].groupby(df['col2']), or by a function which is applied to the index. For example, df.groupby(lambda i: i % 2) groups data by whether the index is even.[4]: 253–259 

Pandas includes support for time series, such as the ability to interpolate values [4]: 316–317  and filter using a range of timestamps (e.g. data['1/1/2023':'2/2/2023'] will return all dates between January 1st and February 2nd).[4]: 295  Pandas represents missing time series data using a special NaT (Not a Timestamp) object, instead of the NaN value it uses elsewhere.

Main Features
Here are just a few of the things that pandas does well:

Easy handling of missing data (represented as NaN, NA, or NaT) in floating-point as well as non-floating-point data
Size mutability: columns can be inserted and deleted from the DataFrame and higher-dimensional objects
Automatic and explicit data alignment: objects can be explicitly aligned to a set of labels, or the user can simply ignore the labels and let Series, DataFrame, etc. automatically align the data for you in computations
Powerful, flexible group-by functionality to perform split-apply-combine operations on data sets, for both aggregating and transforming data
Make it easy to convert ragged, differently-indexed data in other Python and NumPy data structures into DataFrame objects
Intelligent label-based slicing, fancy indexing, and subsetting of large data sets
Intuitive merging and joining data sets
Flexible reshaping and pivoting of data sets
Hierarchical labeling of axes (possible to have multiple labels per tick)
Robust I/O tools for loading data from flat files (CSV and delimited), Excel files, databases, and saving/loading data from the ultrafast HDF5 format
Time series-specific functionality: date range generation and frequency conversion, moving window statistics, date shifting and lagging
Where to get it
The source code is currently hosted on GitHub at: https://github.com/pandas-dev/pandas

Binary installers for the latest released version are available at the Python Package Index (PyPI) and on Conda.

# conda
conda install -c conda-forge pandas
# or PyPI
pip install pandas
The list of changes to pandas between each release can be found here. For full details, see the commit logs at https://github.com/pandas-dev/pandas.

Dependencies
NumPy - Adds support for large, multi-dimensional arrays, matrices and high-level mathematical functions to operate on these arrays
python-dateutil - Provides powerful extensions to the standard datetime module
tzdata - Provides an IANA time zone database
See the full installation instructions for the minimum supported versions of required, recommended and optional dependencies.

Installation from sources
To install pandas from source you need Cython in addition to the normal dependencies above. Cython can be installed from PyPI:

pip install cython
In the pandas directory (same one where you found this file after cloning the git repo), execute:

pip install .
or for installing in development mode:

python -m pip install -ve . --no-build-isolation --config-settings editable-verbose=true
See the full instructions for installing from source.
