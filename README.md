Movie rating

Data source: https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset.

Problem: an online media wants to write an article on the movie ratings over the time, they want to explore what is the overall trend and are there different trends in different Gneres

I imported relevant libraries needed for the project, used pandas to read all the data into a DataFrame.

i had four different file, so i had to combine all the data to form just one dataset 

I checked for missing data and there was a lot of data missing but it was not necessary to drop them as it would not affect the outcome of the project, especially when those missing data are not in the relevant columns and rows.

I found out that the duration of movies has significantly increased over the time, as more movies were produced, the durtion increased from the plot.
Different genres were combined together, this is a problem because we won't be able visualize the actual trend of each genre. So i separated those combined genre by using the EXPLODE() method which transformed each genre to a separate row in the dataset.

I grouped the movies by year and ploted it against average vote, it shows that the average votes received by movies in general have been decreasing from year to year, but that of Biography and sport tend to be more stable with time.
Different Genre was ploted to check if there are different trends for different genre and i found out that generally movie trends have been decreasing over the years but genre Biography and Sport showed to be more stable along 6.0 - 7.0 for Biography and 5.5 - 6.5 for sport.


A linear regression model was biult to predict or show the trend and it showed that generally, the overall movie trend has beeen decreasing over the years with more movies been produced and a longer duration, but that of Genre Biography has been stable over the years with about 6.5 average vote, while that of sport has decreased slightly over the years.

Conclusion: The overall trend of movie ratings is decreasing but a few Genre (Biography and sport) have different trends.
