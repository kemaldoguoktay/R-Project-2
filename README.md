#  📝 Track Genre Suggestion Shiny App

This project is a Shiny app designed to help users discover music genres and tracks based on their preferences for musical attributes such as danceability, loudness, valence, and tempo. The app allows users to explore different genres and tracks and visualize the popularity of different music genres based on selected attributes.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [Authors](#authors)

## Project Overview

This project was developed as part of **Stat295 - Homework 2**. The goal of the project is to apply data visualization and statistical modeling techniques using the R programming language, particularly within a Shiny web application.

The app suggests music genres and tracks based on user-selected intervals for musical attributes. It also allows users to plot the top 10 track genres by popularity and make predictions using a dataset of music tracks.

## Features

- **Musical Attribute Filtering**: Users can select intervals for attributes like danceability, loudness, valence, and tempo.
- **Genre Suggestions**: Based on selected attributes, the app suggests the top 5 matching music genres.
- **Track Suggestions**: After selecting a genre, the app provides a list of tracks sorted by popularity.
- **Genre Popularity Plot**: Users can generate a bar plot displaying the top 10 track genres by popularity.
- **User-Friendly Interface**: The app includes an intuitive UI with sliders and action buttons for easy interaction.

## Installation

To run this Shiny app locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/stat295_hw2.git
   cd stat295_hw2
   ```

2. Ensure you have R and RStudio installed on your machine.

3. Install the required R packages:
   Open RStudio and run the following command to install all necessary libraries:
   ```r
   install.packages(c("ggplot2", "shiny", "tidyverse", "magrittr", "dplyr", "rvest", "httr", "readr"))
   ```

4. Run the app by executing the following in the R console:
   ```r
   shiny::runApp("app.R")
   ```

## Usage

1. **Set Attribute Intervals**: Use the sliders on the sidebar to set your preferred ranges for musical attributes like danceability, loudness, valence, and tempo.
   
2. **Suggest Genres**: Click the `Suggest Genres` button to receive a list of suggested genres that match your selected attributes.

3. **Select Genre**: From the dropdown menu, select a genre for further exploration.

4. **Suggest Tracks**: Click the `Suggest Tracks` button to get a list of popular tracks within the selected genre.

5. **Generate Plot**: Click the `Generate Plot` button to display a plot of the top 10 track genres by popularity.

6. **View and Analyze**: The app will display suggested genres, tracks, and plots based on your input.

### Sample Dataset
The app uses a CSV file containing track details such as:
- `track_id`
- `artists`
- `track_name`
- `danceability`
- `loudness`
- `valence`
- `tempo`
- `popularity`
- `track_genre`

Ensure the dataset (`dataset.csv`) is in the correct format and placed in the app directory.

## Dependencies

The following R packages are required for the app to function:

- **shiny**: For creating the web application interface.
- **ggplot2**: For generating the popularity plot.
- **tidyverse**: For data manipulation and analysis.
- **magrittr**: For the pipe operator (`%>%`) in data processing.
- **dplyr**: For filtering and summarizing the dataset.
- **rvest** and **httr**: For web scraping if needed in future enhancements.
- **readr**: For reading and processing the dataset.

To install these packages, use the command:
```r
install.packages(c("shiny", "ggplot2", "tidyverse", "magrittr", "dplyr", "rvest", "httr", "readr"))
```

## Authors

- **Furkan Kazancıoğlu**
- **Kemal Doğu Oktay**
- **Sefa Bulut**
