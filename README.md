# IMDB exploratory data analysis

## About project
This project used SQL for exploratory data analysis with the IMDB database.
IMDB is the world's most popular and authoritative source for movie, TV and celebrity content. With millions of content listed, IMDB data will provide insights on the content trends, detailed information about TV shows, movies,...

## Database
The database is obtained via this link [https://developer.imdb.com/non-commercial-datasets/]
The database schema is as attached:

![alt text](https://github.com/tamlai-portfolio/SQL-queries-with-IMDB-data/blob/main/ER%20diagram.png)

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
There are 11 types of content listed, the most popular content is TVseries episodes with 839,6170 episodes

2. What year has the most content release?
Aside from content with no listed name, 2021 has 493,044 contents released and is the year with highest number of contents.

3. What is the oldest listed content for each type of content?
The oldest content for movie is Miss Jerry started in 1894
The oldest content for TVseries is Solser en Hesse started in 1900

4. What are the movie genres that has the highest number of released contents?

The movie genres that have the highest number of content:
- Drama has 127,382 contents listed
- Documentary has 102,978 contents listed
- Comedy has 47,814 contents listed
- Horror has 18,214 contents listed
- Thriller has 15,786 contents listed

5. What are top 5 movie genres with most content released last 5 years?
From 2019 to 2024, the top 5 most popular genres of movie are still the overall top 5 of Documentary, Drama, Comedy, Thriller, and Horror, though the ranking of popularity can be a bit diffent in each year.

6. What TV series genres are the most popular in terms of quantity?
Comedy, Drama, Documentary, Reality-TV, Talk-show respectively are the most popular TVseries genres

7. How many genre are there?
There are 2376 different genres listed on IMDB. As there are some genres are duplicated or repeated in a list like (Adventure,Animation,Drama), the number of genres seems to be oddly high.

8. What series has the longest production time from start to end?
If not taking into account those TVseries that is still going on, the longest production time is Mickey Mouse Classic Shorts (85 years from 1928 to 2013)

9.  What are top 5 tv series has highest number of episodes? How many episodes each?
- NRK Nyheter with 18593 episodes
- Days of Our Lives	with 14904 episodes
- General Hospital with 13412 episodes
- As the World Turns with 13339 episodes
- The Young and the Restless with 13046 episodes
These shows are on-going contents with very early startyear.

10.  Top 5 movies has the highest number of votes and highest rating?
- The Shawshank Redemption 
- The Dark Knight
- Inception
- Fight Club
- Forrest Gump

11. What are the movie genres has the highest number of voting? Highest average rating?
Avearage rating for a genres is calculated as weighted average taking into account the number of votes and the total voting points. The list below is order by the total voting points (number of vote * average rating point)
- **Adventure,Animation,Drama**	with 7.74 average rating points
- **Action,Comedy,Documentary**	with 6.80 average rating points
- **Adventure,Mystery,Sci-Fi** with 6.84 average rating points
- **Action,Family,Sport** with 6.10 average rating points
- **Horror,Mystery,Thriller** with 6.39 average rating points


12.  What TV shows have the highest number of votes aggregating from all episodes?
Based on total voting points order:
- Game of Thrones is the tv shows have highest number of votes with 4,483,168 votes and average overall series rating is 8.39
- Attack on Titan is the tv shows have hightest average rating points with 3,058,469 votes and average overall series rating is 9.22
