# Running csv_importer

Default is running in current directory.

## Python version

Use Python 3 (tested with Python 3.6).

## Datasets

Imports [Kaggle movies dataset](https://www.kaggle.com/rounakbanik/the-movies-dataset),
converts to Pandas dataframes with cleanup and exports as pickle files.

Script expects all 6 datasets (*credits.csv*, *keywords.csv*, *links.csv*, *links_small.csv*, *movies_metadata.csv*, *ratings_small.csv*).

## Dependencies

* pandas (with numpy)

## Setting path to movies datasets

```
python csv_importer.py --path /home/ayla/movies
```

## Usage

```
python csv_importer.py --help
```

## Loading Pickle files

Using Python:

```
import pickle

credits_df = pickle.load( open('credits.p', 'rb') )
```

Using pandas:

```
import pandas

credits_df = pandas.read_pickle('credits.p')
```
