# Pandas-

<img width="853" height="367" alt="image" src="https://github.com/user-attachments/assets/2f6c4b86-ea5b-44d5-874a-e935772e2ca7" />



<img width="1049" height="336" alt="image" src="https://github.com/user-attachments/assets/b6e7d04a-4e1f-456a-800d-ca1aeb6c820d" />



Pandas is a core library for data science and data analysis in Python, providing intuitive and flexible data structures, such as the DataFrame. It simplifies the process of data cleaning, manipulation, and analysis, making it an essential tool for anyone working with data.

Main Features
Here are just a few of the things that pandas does well:

Easy handling of missing data (represented as NaN, NA, or NaT) in floating point as well as non-floating point data
Size mutability: columns can be inserted and deleted from DataFrame and higher dimensional objects
Automatic and explicit data alignment: objects can be explicitly aligned to a set of labels, or the user can simply ignore the labels and let Series, DataFrame, etc. automatically align the data for you in computations
Powerful, flexible group by functionality to perform split-apply-combine operations on data sets, for both aggregating and transforming data
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
