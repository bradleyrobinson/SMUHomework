# Assignment 5 CodeBook
## Data
Two raw datasets were used for this assignment: "yob2015.txt" and "yob2016.txt". Each one contains a list of popular baby names for the year, whether they are male or female, and their frequency. The raw data do not include headers.

"yob2015.txt" is essentially a csv file, except it uses ';' as the separating character. "yob2016.txt" is a csv file.

## Objects

df: a dataframe read in from the raw data from yob2016.txt. Has three columns that are manually added: "name", "gender", and "freq".

incorrect\_name: According to instructions there is a row that has the wrong name with three of the letter y in a row. That is found and represented with incorrect\_name.

y2016: The y2016.txt after being cleaned by adding columns and removing the incorrect name.

y2015: The y2015.txt dataframe read in raw. Since this data was clean, this only needs column names added to it. These are the same as y2016.

final: The dataframes y2016 and y2015 merged together by name and gender. Only names that are in both datasets are included. Adds the column 'Total', which includes the total frequency from both years for each name. Also, the column 'freq' is kept separate by year, so the columns "freq\_2016" and "freq\_2015" are added.

sorted: Final sorted in descending order to show which are the most popular names.

just\_girls: The sorted dataframe, but only with girl names.

top\_10\_girls: The top 10 names in top\_10\_girls.

