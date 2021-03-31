# stat-4351-project
## team name, members and responsibilities
The Applied Linear Modelers
Alondra Ramos | introduction of scientific question, future direction, report and presentation organization
Ajay Palankar | regression modeling (statistics heavy)
Courtney Schaller | data visualization (figures and tables)

## dataset
Courtney's 100 Spotify Top Songs 2020 Playlist (Created by Spotify)
This dataset has 15 classes and 100 instances. The Spotify API has several features of every song on the platform. The dataset is available at https://github.com/alondra170/stat-4351-project/blob/main/Courtney's%20Spotify%20Top%20Songs%202020.

### variable descriptions 
pulled from https://developer.spotify.com/documentation/web-api/reference/#endpoint-get-audio-features

Variable Name | Type | Description
--- | --- | --- 
title | string | song title
artist | string | artist name
top genre | string | most likely genre according to Spotify
year added | int | year released
date added | date | date this song was added to the Top Songs 2020 Playlist; as this playlist was automatically created by Spotify, the date is the same for all songs
bpm | int | song tempo in beats per minute
nrgy | numeric | Energy is a measure from 0.0 to 1.0 and represents a perceptual measure of intensity and activity. Typically, energetic tracks feel fast, loud, and noisy. For example, death metal has high energy, while a Bach prelude scores low on the scale. Perceptual features contributing to this attribute include dynamic range, perceived loudness, timbre, onset rate, and general entropy.
danceability | numeric | Danceability describes how suitable a track is for dancing based on a combination of musical elements including tempo, rhythm stability, beat strength, and overall regularity. A value of 0.0 is least danceable and 1.0 is most danceable.
dB | numeric | The overall loudness of a track in decibels (dB). Loudness values are averaged across the entire track and are useful for comparing relative loudness of tracks. Loudness is the quality of a sound that is the primary psychological correlate of physical strength (amplitude). Values typical range between -60 and 0 db.
live | numeric | Detects the presence of an audience in the recording. Higher liveness values represent an increased probability that the track was performed live. A value above 0.8 provides strong likelihood that the track is live.
valence | numeric | A measure from 0.0 to 1.0 describing the musical positiveness conveyed by a track. Tracks with high valence sound more positive (e.g. happy, cheerful, euphoric), while tracks with low valence sound more negative (e.g. sad, depressed, angry).
dur | int | duration of track in seconds
acous | numeric | A confidence measure from 0.0 to 1.0 of whether the track is acoustic. 1.0 represents high confidence the track is acoustic.
spch | numeric | Speechiness detects the presence of spoken words in a track. The more exclusively speech-like the recording (e.g. talk show, audio book, poetry), the closer to 1.0 the attribute value. Values above 0.66 describe tracks that are probably made entirely of spoken words. Values between 0.33 and 0.66 describe tracks that may contain both music and speech, either in sections or layered, including such cases as rap music. Values below 0.33 most likely represent music and other non-speech-like tracks.
pop | numeric | The popularity of a track is a value between 0 and 100, with 100 being the most popular. The popularity is calculated by algorithm and is based, in the most part, on the total number of plays the track has had and how recent those plays are. Generally speaking, songs that are being played a lot now will have a higher popularity than songs that were played a lot in the past.

### response and predictor variables

## data analysis plan
