# Movies-ETL

## Overview
The purppose of this project is to demonstrate the data pipeline process or ETL, Extract Transform & Load.  There are 3 source files:
* movies_metadata.csv
* ratings_csv
* wikipedia.movies.json

In this project, we create a function to read in the three files.  From within that function, we convert to Pandas DataFrames to clean various data elements either with another cleaning function where we iterate through the data elements or we use list comprehensions that filter or modify data elements with regular expressions.

Once our DataFrames are clean, we then merge them and prepare them to be loaded into a Postgres database for further analysis within Postgres.  Our final merged DataFrames includes a Movies table of more than 6,000 records.  A Ratings table is also created that has 26 Million rows.

