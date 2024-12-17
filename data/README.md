# Data Folder

## Folders

We got our Spotify data from Kaggle

Source data:
https://www.kaggle.com/datasets/muhmores/spotify-top-100-songs-of-20152019?resource=download

### Raw

Original, unmodified data after downloading, scraping, etc. 

Description of csv files: 

- The chunk files are the csv files we used to split up the scraping
- The top song streams file is a single file of all of the chunk files
- The api songs file is the data we collected from the api
- The top 1000 songs file is the csv file we downloaded from Kaggle

### Final

Data after all cleaning, processing, and analyzing

Description of csv file:

- This final song csv file includes the cleaned and merged versions of the api file, top 1000 songs file, and top song streams file

---

## Data dictionary

| **Column**       | **Type**     | **Source**       | **Description**                                                            |
|------------------|-------------|------------------|---------------------------------------------------------------------------|
| title            | Text        | Kaggle           | Song’s title                                                              |
| artist           | Text        | Kaggle           | Song’s artist                                                             |
| genre            | Text        | Kaggle           | Genre of the song                                                         |
| year_released    | Date        | Kaggle           | Year the song was released                                                |
| added            | Date        | Kaggle           | Day song was added to Spotify’s Top Hits Playlist                         |
| bpm              | Numeric     | Kaggle           | (Beats Per Minute) - The tempo of the song                                |
| nrgy             | Numeric     | Kaggle           | (Energy) - How electric the song is                                       |
| dnce             | Numeric     | Kaggle           | (Danceability) - How easy it is to dance to the song                      |
| dB               | Numeric     | Kaggle           | (Decibel) - How loud the song is                                          |
| live             | Numeric     | Kaggle           | How likely the song is a live recording                                   |
| val              | Numeric     | Kaggle           | How positive the mood of the song is                                      |
| dur              | Numeric     | Kaggle           | Duration of the song                                                      |
| acous            | Numeric     | Kaggle           | How acoustic the song is                                                  |
| spch             | Numeric     | Kaggle           | The more the song is focused on a spoken word                             |
| pop              | Numeric     | Kaggle           | Popularity of the song (not a ranking)                                    |
| top_year         | Date        | Kaggle           | Year the song was a pop hit                                               |
| artist_type      | Text        | Kaggle           | Tells if artist is solo, duo, trio, or in a band                          |
| streams          | Numeric     | Spotify          | How many people listened to the song                                      |
| pop_today        | Numeric     | Spotify API      | Popularity of the song today (according to Spotify metrics)               |
| Track_id         | Text        | Spotify API      | Each song’s specific identifier at the end of their URL                   |
| url              | Text (url)  | Spotify API      | Specific URL for each song in the data                                    |
