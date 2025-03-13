# Spotify_Popularity

# F23_Project

## Overview

**F23_Project** is an R Markdown project that performs statistical analysis on Spotify music data. It utilizes data processing, visualization, and regression modeling techniques to explore relationships between various song attributes and their popularity on music streaming platforms.

## Author

**Ethan Carter**

## Date

**November 7, 2023**

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset Description](#dataset-description)
- [Project Workflow](#project-workflow)
- [Statistical Analysis](#statistical-analysis)
- [Results and Visualization](#results-and-visualization)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

This project utilizes R Markdown to analyze a dataset containing metadata and popularity metrics of songs from Spotify. The goal is to understand how different musical features correlate with a song’s presence on streaming charts.

## Installation

To run this project, ensure you have the following dependencies installed in R:

```r
install.packages("dplyr")
install.packages("lmtest")
install.packages("MASS")
install.packages("car")
install.packages("mlr")
```

Additionally, you need R Markdown to generate reports:

```r
install.packages("rmarkdown")
```

## Dataset Description

The dataset contains various song attributes, including:

- **track_name**: Name of the song
- **artist(s)\_name**: Name of the artist(s)
- **released_year, released_month, released_day**: Release date details
- **in_spotify_playlists, in_spotify_charts**: Spotify playlist and chart metrics
- **streams**: Total number of streams
- **bpm, key, mode**: Musical attributes like tempo and tonality
- **danceability*%, valence*%, energy\_%**: Characteristics influencing a song’s vibe
- **instrumentalness*%, liveness*%, speechiness\_%**: Audio and vocal properties

## Project Workflow

### 1. Data Loading & Preprocessing

- Reads data from a CSV file
- Converts raw data into a structured dataframe
- Handles missing values and categorizes variables

### 2. Exploratory Data Analysis (EDA)

- Extracts key variables for analysis
- Computes statistical summaries
- Filters and cleans data

### 3. Statistical Analysis

- Constructs Simple Linear Regression (SLR) models to analyze the impact of tempo, danceability, and energy on Spotify rankings
- Implements a Multiple Linear Regression (MLR) model incorporating multiple variables

## Statistical Analysis

The following statistical tests and transformations were performed:

- **Residual Analysis**: Checking assumptions of normality and homoscedasticity
- **Breusch-Pagan Test**: Detecting heteroscedasticity
- **Box-Cox Transformation**: Addressing normality violations
- **Weighted Least Squares (WLS)**: Handling heteroscedasticity

## Results and Visualization

Several plots and models are generated to analyze relationships:

- **Scatter plots** of song features vs. chart ranking
- **Box plots and histograms** for distribution analysis
- **Regression model summaries** with statistical significance tests

## Conclusion

The project provides insights into the factors influencing a song’s popularity. The analysis suggests that danceability, energy, and tempo have varying degrees of impact on Spotify chart rankings.

## References

For further details on R Markdown and statistical modeling in R, visit:

- [R Markdown Documentation](http://rmarkdown.rstudio.com/)
- [CRAN: The R Project](https://cran.r-project.org/)
