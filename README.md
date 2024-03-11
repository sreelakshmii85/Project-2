Text contains SQL queries and commands related to managing and querying a table named netflix_movies_bkt in a Hive environment. Here's a brief description of the content:

1. *Table Creation and Loading Data*: It begins with the creation of a table named netflix_movies and loading data into it from a CSV file. Then, it creates another table named netflix_movies_bkt partitioned by year and clustered by score.

2. *SQL Queries*: Various SQL queries are performed on the netflix_movies_bkt table to extract specific information:
   - Finding the highest and lowest scored movies.
   - Retrieving the movie title and maximum score for each movie.
   - Selecting movies starting with "Th" and displaying their rank and release year.
   - Listing the top 10 movies with their release year and score.
   - Finding movies directed by "Paul Greengrass" and their cast.
   - Listing movies released in 2019 along with their scores.
   - Listing movie directors whose names start with "Pa".
   - Displaying the last 10 movies from the table along with their scores.

Overall, the text demonstrates SQL commands used for data management and analysis in the context of a Netflix movies dataset stored in a Hive environment.
*create table netflix_movies(rank int,movie_title string,year int,score int,director string,movie_cast string,critics_consensus string)row format delimited fields terminated by ','tblproperties('skip.header.line.count'='1');
*load data local inpath '/home/amitha/data/kaggle_data/100 Best Movies on Netflix.csv' into table netflix_movies;
