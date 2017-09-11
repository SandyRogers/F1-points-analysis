# F1 history: points won during qualifying vs. races
This Jupyter Notebook (Python) analyses the history of F1, in terms of how teams are incentivised.

# Getting the dataset
We use historical F1 data from [The Ergast API](http://ergast.com/mrd/).
The SQL database can be downloaded [here](http://ergast.com/mrd/db/).

To run this analysis, download the database image from Ergast.
Load it into a local MySQL database [(see StackOverflow)](https://stackoverflow.com/questions/17666249/how-to-import-an-sql-file-using-the-command-line-in-mysql)

# What are we analysing?
I wanted to know whether F1 racedays are becoming more or less competitive. I had a feeling that we needed to look at the relative importance of qualifying vs. racedays, in terms of how many points per (effectively) won on each day. The thinking was that: if most points are "already won" in qualifying, teams would make less race-competitive cars (since they only need to be qualifying-competitive).

For more interpretation, check out [this Medium post](https://medium.com/p/4d080f93dc4b).

The result is a graph that looks like this (as of August 2017):
![History of F1 points race novelty](F1%20raceday%20novelty.png)

# Installation
You'll need python, jupyter, jupyter notebook, pandas, matplotlib, numpy, mysqldb.
