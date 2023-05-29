# **Read:12 Summary**

**Pandas**

- pandas is a Python package providing fast, flexible, and expressive data structures designed to make working with "relational" or "labeled" data both easy and intuitive. It aims to be the fundamental high-level building block for doing practical, real world data analysis in Python. Additionally, it has the broader goal of becoming _ **the most powerful and flexible open source data analysis / manipulation tool available in any language** _. It is already well on its way toward this goal.
- Pandas is a game-changer for data science and analytics, particularly if you came to Python because you were searching for something more powerful than Excel and VBA. Pandas uses fast, flexible, and expressive data structures designed to make working with relational or labeled data both easy and intuitive.

_ **pandas is well suited for many different kinds of data:** _

- Tabular data with heterogeneously-typed columns, as in an SQL table or Excel spreadsheet
- Ordered and unordered (not necessarily fixed-frequency) time series data.
- Arbitrary matrix data (homogeneously typed or heterogeneous) with row and column labels
- Any other form of observational / statistical data sets. The data actually need not be labeled at all to be placed into a pandas data structure

_ **The two primary data structures of pandas :** _

- Series (1-dimensional) ( 1D labeled homogeneously-typed array )
- DataFrame (2-dimensional) ( General 2D labeled, size-mutable tabular structure with potentially heterogeneously-typed column )


- Pandas handle the vast majority of typical use cases in finance, statistics, social science, and many areas of engineering
- pandas is built on top of NumPy and is intended to integrate well within a scientific computing environment with many other 3rd party libraries.

_ **Here are just a few of the things that pandas does well:** _

- Easy handling of missing data (represented as NaN) in floating point as well as non-floating point data
- Size mutability: columns can be inserted and deleted from DataFrame and higher dimensional objects
- Automatic and explicit data alignment: objects can be explicitly aligned to a set of labels, or the user can simply ignore the labels and let Series, DataFrame, etc. automatically align the data for you in computations
- Powerful, flexible group by functionality to perform split-apply-combine operations on data sets, for both aggregating and transforming data
- Make it easy to convert ragged, differently-indexed data in other Python and NumPy data structures into DataFrame objects
- Intelligent label-based slicing, fancy indexing, and subsetting of large data sets
- Intuitive merging and joining data sets
- Hierarchical labeling of axes (possible to have multiple labels per tick)
- Robust IO tools for loading data from flat files (CSV and delimited), Excel files, databases, and saving / loading data from the ultrafast HDF5 format
- Time series-specific functionality: date range generation and frequency conversion, moving window statistics, date shifting and lagging.


- pandas is a dependency of statsmodels, making it an important part of the statistical computing ecosystem in Python.
- pandas has been used extensively in production in financial applications.
- DataFrame is a container for Series, and Series is a container for scalars. We would like to be able to insert and remove objects from these containers in a dictionary-like fashion.
- All pandas data structures are value-mutable (the values they contain can be altered) but not always size-mutable. The length of a Series cannot be changed, but, for example, columns can be inserted into a DataFrame
- _ **To start using pandas :** _ import pandas as pd
- Each column in a DataFrame is a Series


**The most elementary functions of pandas**

- Reading data : data = pd.read\_csv('my\_file.csv')
- Writing data : data.to\_csv('my\_new\_file.csv', index=None)
- Checking the data : data.shape OR data.describe()
- Seeing the data : data.head(3) OR data.loc[8] OR data.loc[8, 'column\_1'] OR data.loc[range(4,6)]

**The basic functions of pandas**

- Logical operations :
  - data[data['column\_1']=='french']
  - data[(data['column\_1']=='french') & (data['year\_born']==1990)]
  - data[(data['column\_1']=='french') & (data['year\_born']==1990) & ~(data['city']=='London')]
  - data[data['column\_1'].isin(['french', 'english'])]
- Basic plotting
  - data['column\_numerical'].plot()
  - data['column\_numerical'].hist()
  - %matplotlib inline/
- Updating the data
  - data.loc[8, 'column\_1'] = 'english'
  - data.loc[data['column\_1']=='french', 'column\_1'] = 'French'

**Medium level functions**

- Counting occurrences
  - data['column\_1'].value\_counts()
- Operations on full rows, columns, or all data
  - data['column\_1'].map(len)
  - data['column\_1'].map(len).map(lambda x: x/100).plot()
  - data.apply(sum)
- Correlation and scatter matrices
  - data.corr()
  - data.corr().applymap(lambda x: int(x\*100)/100)
  - pd.plotting.scatter\_matrix(data, figsize=(12,8))

**Advanced operations in pandas**

- The SQL join
  - data.merge(other\_data, on=['column\_1', 'column\_2', 'column\_3'])
- Grouping
  - data.groupby('column\_1')['column\_2'].apply(sum).reset\_index()
- Iterating over rows
  - dictionary = {}
  - for i,row in data.iterrows():
  - dictionary[row['column\_1']] = row['column\_2']

**Conclusion**

- Panda is simple to use, hiding all the complex and abstract computations behind
- Panda is (generally) intuitive
- Panda is fast, if not the fastest data analysis package (it highly optimized in C)
- It is THE tool that helps a data scientist to quickly read and understand data and be more efficient at his role.