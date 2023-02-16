#  Project 1: Spotify API :headphones:
## Introduction
  Spotify is a “ digital music, podcast, and video service that gives you access to millions of songs and other content from creators all over the world”. As of late 2022, Spotify has 465 million users and is the most popular music streaming service. Spotify has curated playlists for a large variety of genres and playlists for top 50 popular songs in each country. 

##  GOALS / DELIVERABLES
 Our first goal overall was to connect to the api. We did this through a python library that speically is used for connecting to the spotify API. It made it simple and seamless to connect our keys and start quering the API.
 Our next goal was to extract our insights into a Dataframe. This was done by connecting many of the API endpoints together to create one dataframe we were able to manipulate.
 From there we gathered out insights. Creating data and graphs for each specific question:
 *  For the regression we used the top 50 global playlist. We chose popularity as the dependent variabel and used the other attributes to analyze if there was any correlation between them. This included genres which we needed to create dummy variables for to be able to add it to the regression model.
  * Our next question invloved the Top 100 playlists from every 5 years between 1970 and 2023. We looked at the mean of each attribute and created line graphs to visually see how those numbers have changed from year to year. We also included pie charts to see how the genere popularity changed year to year.
  * Lastly, we looked at genre distrobution from before the 2019 pandemic to after. This allowed us to see how music tastes have changed since then and try to draw some insights on if quarentine played a roll in those changes.

 ## Tools used to analyze 
 - Spotify Api
 - Python
 - Jupyter Notebook

##  AUDIO FEATURE DEFINITIONS
 Its important to know what each attribute mean and how they are categorized within the Spotify API.
* Acousticness - A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
* Danceability - Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
 * Energy - Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
* Instrumentalness - Predicts whether a track contains no vocals. “Ooh” and “aah” sounds are treated as instrumental in this context. Rap or spoken word tracks are clearly “vocal”. The closer the instrumentalness value is to 1.0, the greater likelihood the track contains no vocal content. Values above 0.5 are intended to represent instrumental tracks, but confidence is higher as the value approaches 1.0.
* Liveness - Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
* Loudness - The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typically range between -60 and 0 db.
* Speechines - Detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
* Valence - A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
-----------------------------------------------------------------------------------------------------------------------
# Analysis

## Regression Conclusion
   When it came to the regresion, the conclusion that could be drawn is that there is little effect on popularity based off the given attributes. In fact genres had more of a impact then the given audio atributes.

## How has popular music changed over the last 50 years? 
  For the changes over the last 50 years, we looked at four specific audio features.
    
* Danceability - there was an increase over the last 50 years. This can be indicated by a rise in latin music, caribbean music and also hip hop and rap.
    
* Valence - this category has been decreasing for the last 50 years. This can be due to a number of societal reasons. First, around 1980 thhere was a sharp decline in religious people. This may have an affect on what kind of music is tolerated. Music also became more blunt and spoke about real world issues, most of with were not happy. Finally, this may be due to just artists setting the trend for those to come. People continue to raise the bar, with each wave of popular artists, on how sad music can be.
   
* Speechiness - this category has overall been rising since 1985, with occasional dips around 2015 and 2021. The rapid rise in speechiness around 1990 can be attributed to the growing rap scene. There was a lot of competition between east and west coast rappers, this drove song production and then the poularity with rap overall.
    
* Explicit - songs that are explicit have been on the rise since 1990. This again can be attributed to the rise of rap, also the idea that hip hop and r$b were on the rise. There was less pressure by record labels to give out a clean and polished song. Society was craving raw truth and music provided that
