![](https://miro.medium.com/max/1296/1*8nj0WVUjsu5vhQdYyVY7Fg.jpeg)

# Do Attributes of Songs on Spotify Correlate to a Song's Popularity?

[Introduction](#Introduction)

[Technologies Used](#Technologies-Used)

[What's in the Data?](#What's-in-the-Data?)


## Introduction
There's a time when we listen a song, and the only thing that can be said is, "This is a hit"! What truly attracts us to certain sounds, and gets us hooked immediately? We'll take a deep dive into a vast collection of songs on Spotify, look at the songs' attributes, and find correlation of those attributes to the songs' popularity.

<br>

## Technologies Used
* *Pandas*
* *NumPy*
* *Scipy*
* *Matplotlib*

<br>

## What's in the Data?
This dataset contains a collection of 174,389 songs from the Spotify API that a user on [Kaggle](https://www.kaggle.com/yamaerenay/spotify-dataset-19212020-160k-tracks), with publishing spanning from 1920 to 2021. We'll focus on a subset of the data that spans from 2000 to 2021, narrowing it down to 40,531 songs, and keeping our analysis spotlight on modernity. Each row represents a song and its features. We'll define the features of focus, and what each of them means and represents further down. All of this data is in a CSV file.

<br>

## Exploratory Data Analysis
I created a subset of the data to keep it relevant to current trends from the year 2000 to 2021. I cleaned it up to only analyze my columns of interest, which are:

<br>

[Popularity]()

[Danceability]()

[Energy]()

[Instrumentalness]()

[Speechiness]()

[Explicit]()

[Mode]()

<br>

### Features of Focus as Popularity Goes Up
|**POPULARITY** |artists|name|Danceability |Energy |Instrumentalness |Speechiness |Explicit |Mode |
|:--------------|:-------|:----|:------------:|:------:|:----------------:|:-----------:|:--------:|:----:|
|         **30**| ['Robin Trower']|Farther on up the Road - 2012 Remaster| 0.469|  0.918|         0.000392|      0.1730|        0|    1|
|         **30**| ['Armin van Buuren']|A State Of Trance (ASOT 996) - Tune Of The Yea...| 0.397|  0.638|         0.000000|      0.1760|        0|    1|
|         **30**| ['Above & Beyond', 'Zoë Johnston']|Reverie - Above & Beyond Club Mix| 0.453|  0.756|         0.064800|      0.0472|        0|    1|
|...            |...    |    |...      |...    |...              |...         |...      |...  |
|         **95**| ['KAROL G']|BICHOTA	| 0.863|  0.666|         0.000493|      0.1520|        1|    0|
|         **96**| ['Ariana Grande']|positions	| 0.737|  0.802|         0.000000|      0.0878|        1|    1|
|         **96**| ['24kGoldn', 'iann dior'] |Mood (feat. iann dior)| 0.700|  0.722|         0.000000|      0.0369|        1|    0|


Above, you'll se we sorted the data by *Popularity* in ascending order from **30** to **100**, dropping it down to **22,030 rows x 9 columns**.

<br>

### Popularity
> **Spotify Popularity** is an extremely important value that Spotify uses internally to rank all tracks on **a scale from 0 to 100**.
<br>
It lets you see how the Spotify algorithm currently evaluates you and your music. The higher your popularity index, the more likely the algorithm is to recommend you to new listeners, and place you in algorithmic playlists like *Release Radar* and *Discover Weekly*.

