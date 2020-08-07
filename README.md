# ETL-Project
For our ETL Project, we decided to take a look at a large, multi .CSV dataset about the Police violence.  We found this dataset on Kaggle at https://www.kaggle.com/jpmiller/police-violence-in-the-us.  This data set contained a total of 22 csv files, but by looking at the files, we narrowed them down to 11 files.

To be able to use these files, there was some data transformation that had to take place.  4 of the files   contained the same information, but for different years so we merged the csv files with a concat function.  From there we cleaned the data to the columns that we deemed as useful.  For most of the files, if there was no information entered in a field, we replaced it with a zero or dropped the column all together.

Once the data was translated, we loaded the csv files into a database with different collections for each of the files.  We decided to use a non-relational database and used MongoDB to store our database and collections.
