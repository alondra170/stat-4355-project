# stat-4355-project
## Team name, members and responsibilities
The Applied Linear Modelers
Team Member | Responsibility
--- | ---
Alondra Ramos | Regression modeling, residual analysis, and residual visualizations
Ajay Palankar | Introduction of scientific question, future direction, report and presentation organization, some data visualizations
Courtney Schaller | Variable selection, data visualization, model analysis

## dataset
Rolling Stone's 500 best albums of all time on Spotify from the year 2020 (see the list here: https://www.rollingstone.com/music/music-lists/best-albums-of-all-time-1062063/) 
This dataset has 15 classes and 6657 instances. The Spotify API has several features of every song on the platform. The dataset is available at https://github.com/alondra170/stat-4351-project/blob/main/Courtney's%20Spotify%20Top%20Songs%202020.

## data description
For our project, we chose to analyze a dataset of Rolling Stone's 500 best albums of all time on Spotify from the year 2020. This dataset took all the songs from Rolling Stone's best albums list and compiled it into a big playlist. In particular, the dataset involves multiple numerical and categorical variables which help the user understand the components of each song. Such components include Spotify's algorithms' best estimates of whether a song was created in front of a live audience, how popular a song is, and a song's positivity. Most importantly, our group will focus on how the energy of a song is impacted due to variables such as the danceability, popularity, and acousticness variables. We chose to focus on the energy of a song as our goal of study because we believe studying energy will allow for both audiences and artists to have a clear, objective understanding of what makes a song high- or low-energy. In addition, studying popularity will allow us to gain insight into clear, yet detailed understanding of the mathematical and statistical relationships between the variables of the Spotify dataset.

### variable descriptions 
confirmed with https://developer.spotify.com/documentation/web-api/reference/#endpoint-get-audio-features

Variable Name | Name in Dataset | Type | Range in Dataset | Description
--- | --- | --- | --- | ---
Title | title | string | | song title
Year Added | year added | int | 1955-2019 | year released
Tempo | bpm | int | 0-244 | Tempo of a track in beats per minute. A high tempo indicates a fast song, a low, a slow song.
Energy | nrgy | numeric | 0-100 | Energy is on a 0-100 scale and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
Danceability | danceability | numeric | 0-98 | Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0 is least danceable and 100 is most danceable.
Loudness | dB | numeric | -60-0 | The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range between -60 and 0 db.
Live | live | numeric | 0-100 | Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
Positivity | valence | numeric | 0-99 | A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
Duration | dur | numeric | 4-947 | duration of track in seconds
acous | numeric | 0-100 | A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
Speech | spch | numeric | 0-96 | Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
Acousticness | acous | numeric | 0-100 ? The acousticness of a track is a value between 0 and 100, with 100 being the most "acoustic" track possible. 
Popularity | pop | numeric | 0-92 | The popularity of a track is a value between 0 and 100, with 100 being the most popular. The popularity is calculated by algorithm and is based, in the most part, on the total number of plays the track has had and how recent those plays are. *Generally speaking, songs that are being played a lot now will have a higher popularity than songs that were played a lot in the past.*

### response and predictor variables

Response Variable: Energy / nrgy (numeric)

Predictor Variables:
  
    Year Released / year added (int)
    Beats Per Minute / bpm (numeric)
    Danceability / danceability(numeric)
    Loudness / dB (numeric)
    Live / live (numeric)
    Happiness / valence (numeric)
    Duration / dur (numeric)
    Acousticness / acous (numeric)
    Speechiness / spch (numeric)

## analysis goal

Our goal for this study is to determine how various predictor variables of a song such as when the song was published, its tempo, popularity, and danceability impacts the energy level of a song. Specifically, to determine whether each individual predictor variable affects popularity, and if so, to what degree it increases or decreases it. This could help songwriters determine how to write a high-energy track, or help spotify understand trends across songs and across genres. With temporal features such as Year Released, we can see whether or not music has grown more or less energetic over time. With features like Happiness we can see whether happier songs tend to have more energy.

## data analysis plan

Data exploration and cleaning will be implemented by extracting the chosen predictor variables, handling null values, as well as exploring the data through plots and looking at summary statistics to ensure the distribution of our predictor variable is balanced and appropriate to create a useful model. We will also investigate the predictors and weed out any instances of colinearity among them to ensure the model creation is giving meaningful insight to regressor significance. 

The next phase consists of model construction with the linear regression functions provided in R. The first model will consist of all of the listed predictors post-cleaning. From there numerous metrics and figures such as RSE, R^2, p-values, error plots and others will be examined for fit and appropriateness with implications and conclusions documented accordingly. Experimentation with different forms of the model will be executed after considering the significance of each regressor and other factors. This will repeated until sufficient and satisfactory insights into the data are achieved. Figures and tables will be constructed to summarize and visualize results and a future direction will be decided accordingly.
