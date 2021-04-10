![](https://i.guim.co.uk/img/media/ae483ce4f1bfc5497fee1b5387711d1ff0172ec9/232_0_3268_1963/master/3268.jpg?width=1200&quality=85&auto=format&fit=max&s=fcfceea59329a6bee9c9b75dd8d7a055)

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
This dataset contains a collection of 174,389 songs from the Spotify API, with publishing spanning from 1920 to 2021. We'll focus on a subset of the data that spans from 2000 to 2021, narrowing it down to 40,531 songs, and keeping our analysis spotlight on modernity. Each row represents a song and its features. We'll define the features of focus, and what each of them means and represents further down. All of this data is in a CSV file.

<br>

## Exploratory Data Analysis
I created a subset of the data to keep it relevant to current trends from the year 2000 to 2021. I cleaned it up to only analyze my columns of interest, which are:<br>

[Popularity]()

[Danceability]()

[Energy]()

[Instrumentalness]()

[Speechiness]()

[Explicit]()

[Mode]()

<br>

## Features to analyze Correlation as Popularity goes up 
|popularity |danceability |energy |instrumentalness |speechiness |explicit |mode |
|:----------|------------:|------:|----------------:|-----------:|--------:|----:|
|         30|        0.469|  0.918|         0.000392|      0.1730|        0|    1|
|         30|        0.397|  0.638|         0.000000|      0.1760|        0|    1|
|         30|        0.453|  0.756|         0.064800|      0.0472|        0|    1|
|         30|        0.912|  0.701|         0.000000|      0.0744|        1|    1|
|         30|        0.591|  0.625|         0.000000|      0.3080|        0|    1|

<br>