# Movies Data - EDA

### Objective - Exploratory Data Analysis on Movies data to understand what all factors affect Revenue in a Movie.

   ![](https://github.com/mihirjain08/project/blob/main/Images/online-cinema-art-movie-watching-260nw-584655766.jpg?raw=true)

The movie industry consists of various establishments whose major engagements are the marketing and circulation of audiovisual pieces to TV networks and movie theaters. The film industry is made up of the commercial and technological filmmaking companies. These film industry companies may include production, screenwriting, film studios, and cinematography, among other endeavors.

- The box office is a measurement of the total gross of tickets sold for a particular movie, essentially the revenue from ticket sales. 
- In the film industry, box office sale values are significant in order to assess how successful a movie is. For film studios, box office numbers are important for potential future projects.

On a worldwide scale, the North American box office market leads by a significant amount compared to other markets. 

- In 2019, box office revenue in the United States and Canada amounted to 11.4 billion U.S. dollars.
- In the U.S. and Canada, the average cost of a movie ticket amounted to 9.16 U.S. dollars in 2019, up from 9.11 dollars in the previous year. 
- Prices have been on the increase since 2001, when a movie ticket cost 5.66 dollars on average.

------------


### Problem Statement

- Cinemania, an American Box Office where tickets are sold to the public for movies.

- Over the past few years, it has become one of the most liked and visited place in different areas.

- They are planning to add new services and enhance the quality of existing services.

- I will be working independently on the dataset available to understand what are the factors which governs revenue generation and give my conclusion and insights.

------------

### Dataset

|  Feature | Description  |
| :------------: | :------------: |
| Rank  |  Movie Rank |
| Title  | Title of the movie  |
| Genre  |  The various Genre that the movie can be associated with |
| Description  | Short description about the movie  |
| Director  | Director of the movie  |
| Actors  | Main actors in the movie  |
| Year  | Year in which the movie was released  |
| Runtime (minutes)  | Total movie playing time  |
| Rating  | Movie rating  |
| Votes  | Votes for the movie  |
| Revenue (Millions)  | Revenue by the movie (in millions)  |
|  Metascore | Is the score of the movie on the metacritic website by critics  |


------------

### Pandas Profiling

Based on the Pandas Profiling, here are some of the observation of the dataset

- Genres - It gives us the info that 'Action, Adventure, Scifi, Drama, Comedy' are the most watched genres.
- Year - Data contains from 2006 to 2016
- Runtime (minutes) - It varies from 66 min to 192 min. Avg runtime is 113 minutes. 50% of the movies in this dataset have runtime in between 100 to 123 minutes.
- Rating - Minimum rating is 1.9 and amx rating is 9. 50% of the dataset have rating varying from 6.2 to 7.4
- Votes - Minimum votes given to a movies is 61 and max votes received by a movies is 1791916 votes.
- Revenue - 128 missing values. Lot of outliers on the higher side. Highest revenue is 936.63 millions
- Metascore - 64 missing values

Interaction between variables

- Rating and votes doesn't seem to be correlated with each other.
- Rating and metascore have correlation

Pearson's correlation

- It suggest the same - Rating and metascore have high correlation - means critics rating and people's rating have some correlation
- Revenue and votes have high correlation - Means movies with high revenue will have high vote count
- Rating and revenue have low correlation value


------------

### Conclusion

- Movies with a lot of votes (over 1o millions) are a rarity, with the number of votes dropping the number of films also drops.

- There is a big difference between the maximum and minimum runtime of popular movies, based on genre.

- New movies are more popular than old movies as observed in the dataset.

- Rating and Metascore are quite similar, however, metascore is somewhat more uniformly distributed than rating.

- Most popular movies last between 100 and 123 minutes.

- Only few popular movies have high revenues.

- High-rated movies do not give you large incomes or a large number of votes.

- Few genres like Action, adventure, sci-fi, Drama, have higher votes as well as revenues for their titles.

- Actors / director play a big role in getting more no of votes. Their popularity also affects revenue generation.

- Metascore and rating have positive co-relation but votes and rating doesn't


------------

### Actionable Insights

- There has to be a Genre based filter in the application for visitors to choose movies as per their likes

- Every movie which is listed in the app for, it must have few pointers to show Genre, director, Star Cast (lead roles specially the popular ones)

- There should be a news feed tab in the app which gives latest info about some popular movie title, actors and directors info.

- One unique feature we can built in the app is filter based on runtime of a movie. Most people plan their time in a way that they cannot spent 3 hours for movie, based on popular choice, they can select runtime, which will save their time to individually check for movies time on internet.

- We can have a comments section also, if not there, to understand more about what they like and do not like.

- Movies with some specific title, director, actor are popular as seen in votes share, such movies alert shud be created and users can get notification about the same, to engage them with using our platform.

- Lastly, personalized experiance should be provided by notifying the user, your favourite genre, actor, director movie is in theatres, did you watch yet? go ahead and book the tickets.

------------


