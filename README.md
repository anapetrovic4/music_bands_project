# Music Data Collection and Analysis

This project focuses on collecting, cleaning, and analyzing music-related data from multiple online sources, including **Spotify**, **AllMusic**, and **Wikipedia**.  
The workflow consists of web scraping, dataset cleaning, merging datasets from different sources, and performing both descriptive and exploratory analysis.  
The final goal is to build a comprehensive dataset that can be used for deeper insights into artists, bands, and their music.

# Project Structure

## scripts
- **allmusic**
  - data_cleaning
  - data_cleaning_2
  - web_scraping
- **merging_and_cleaning** <br>
Python script implementing the merging and cleaning procedures described in the previous sections
  - final_dataset_merging_and_cleaning

- **spotify**
  - data_cleaning
  - data_cleaning_2
  - data_extraction
  
- **wikipedia**
  - data_cleaning
  - web_scraping

---

## analysis
- **descriptive_analysis**  
  Descriptive statistics as an introduction to exploratory analysis
- **exploratory_analysis**  
  Exploratory analysis applied to the *csny* dataset

---

## data
- **AllMusic Datasets**
  - raw
  - v2
  - v3
- **combined** <br>
Datasets created by combining individual artist/band datasets from different sources:
  - *allmusic-combined*
  - *wikipedia-combined*
  - *spotify-combined* <br>
Dataset created by combining *allmusic-combined* and *wikipedia-combined*:  
  - *allmusic-wikipedia-combined*
  
- **final** <br>
Dataset created by combining *allmusic-wikipedia-combined* and *spotify-combined*
  - csny
- **Spotify Datasets**
  - raw
  - v2
  - v3
- **Wikipedia Datasets**
  - raw
  - v2
  - v3

---
