# IMDB exploratory data analysis

## About project
This project used SQL for exploratory data analysis with the IMDB database.
IMDB is the world's most popular and authoritative source for movie, TV and celebrity content. With millions of content listed, IMDB data will provide insights on the content trends, detailed information about TV shows, movies,...

## Database
The database is obtained via this link [https://developer.imdb.com/non-commercial-datasets/]
The database schema is as attached:

![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)

## Analysis process

### Data cleaning
A - Movie table:
- [x] Convert runtimeMinutes to number and replace /N with null values
- [x] Convert startYear and endYear into numberic type with /N is null values

B - Actor table:
- [x] Convert the deathYear of /N to null values

C - Episode table:
- [x] Convert the /N to null values

### Exploratory questions to answer:

1. What are the type of contents listed on imdb? How many?
2. What year has the most content release?
3. What is the oldest listed content for each type of content?
4. What are the genres that has the highest number of released contents?
5. What are top 5 movie genres with most content released last 5 years?
6. What TV series genres are the most popular in terms of quantity?
7. How many genre are there?
8. What series has the longest production time from start to end?
9. What are top 10 tv series has highest number of episodes? How many episodes each?
10. Top 10 movies has the highest number of votes and highest rating?
11. What are the movie genres has the highest number of voting? Highest average rating?
12. What TV shows have the highest number of votes aggregating from all episodes? 
