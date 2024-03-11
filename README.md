*create table netflix_movies(rank int,movie_title string,year int,score int,director string,movie_cast string,critics_consensus string)row format delimited fields terminated by ','tblproperties('skip.header.line.count'='1');
*load data local inpath '/home/amitha/data/kaggle_data/100 Best Movies on Netflix.csv' into table netflix_movies;
