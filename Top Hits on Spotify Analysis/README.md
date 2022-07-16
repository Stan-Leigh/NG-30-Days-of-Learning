# Analysis of Top Hits on Spotify

## Introduction
This report analyzes the audio statistics of the top 2000 tracks on Spotify from 1998 to 2019. All the analyses was performed in Microsoft PowerBI.

The dataset was collected from [Kaggle](https://www.kaggle.com/datasets/paradisejoy/top-hits-spotify-from-20002019). 
It contains 18 columns that describes the track and its qualities. The columns consists of:
* artist (name of the artiste)
* song (name of the song)
* duration_ms (duration of the track in milliseconds)
* explicit (whether the content of the song is unsuitable for children)
* year (release year of the track)
* popularity (The higher the value, the more popular the song is)
* genre (the genre of the track)

and a host of others.

## Data Wrangling
The dataset was cleaned from the get-go but some minor modifications were made in Power Query:
* Formatted the duration_ms column to represent how long the song lasted in minutes and seconds.
* Converted the year and popularity columns to Date and Integer datatypes respectively.
* Created a new index column to serve as a primary key column for the dataset.

## Observations
* There are **835** artistes in this dataset.
* **Rihanna** is the most popular artiste, producing the highest number of hit songs, **25**.
* **Sweater Weather** produced by **The Neighborhood** has the highest popularity rating.
* The most popular genres are **pop**, **hip hop**, **R&B** and **Dance/Electronic**.
* Year 2018 had the highest average popularity, **70.85**.
