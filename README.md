# Spotify_project

In this project, I built a Spotify recommendation engine, it ask you for a song and it tells you if it is a hot song or not, if not it ask you for a play list that you like and based on it, it recommends you a song that probably you will like taking into account the first song that you told to the program.

**To do it a follow three main steps.**

1.	Web scraping from the top100 songs from a website called Billboard. Specifically retrieving the title and artist of those hits. This information will later on be useful as the recommendation engine will advise a user to listen to a random current hit song in the top 100 if the query has been another hit song.

2.	By using the Spotify API Wrapper, I made a function which if you write the link of a playlist, first it take all the singers of this play list, secondly it takes all songs from the singers of the play list and with this information it builds a data set, the last step of budling the data set is to drop duplicates (there can be repeated songs).
The data set contains information about the singers, songs and audio features (e.g. Danceability, Loudness...).

3.	Finally I build, through the usage of an unsupervised machine learning model, a recommendation engine which will receive an input (a title of any songs currently on Spotify) and will advise either a top 100 song (if the input song was in the top 100 of Billboard), or a similar song in terms of audio feature based on a play list that you like.

![](images/spotify.jpg)
