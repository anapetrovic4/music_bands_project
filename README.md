# Music Data Collection and Analysis

This project focuses on collecting, cleaning, and analyzing music-related data from multiple online sources, including **Spotify**, **AllMusic**, and **Wikipedia**.  
The workflow consists of web scraping, dataset cleaning, merging datasets from different sources, and performing both descriptive and exploratory analysis.  
The final goal is to build a comprehensive dataset that can be used for deeper insights into artists, bands, and their music.

# Project Structure

The repository is organized as follows:
```
.
├── analysis/                     # Analysis notebooks
│   ├── descriptive_analysis.ipynb
│   └── exploratory_analysis.ipynb
│
├── data/                         # All datasets
│   ├── AllMusic/
│   │   ├── raw/
│   │   ├── v2/
│   │   └── v3/
│   │
│   ├── Spotify/
│   │   ├── raw/
│   │   ├── v2/
│   │   └── v3/
│   │
│   ├── Wikipedia/
│   │   ├── raw/
│   │   ├── v2/
│   │   └── v3/
│   │
│   ├── combined/                 # Combined datasets
│   │   ├── allmusic-combined/
│   │   ├── wikipedia-combined/
│   │   ├── spotify-combined/
│   │   └── allmusic-wikipedia-combined/
│   │
│   └── final/                    # Final dataset
│       └── csny/
│
├── scripts/                      # Python scripts
│   ├── allmusic/
│   │   ├── data_cleaning.py
│   │   ├── data_cleaning_2.py
│   │   └── web_scraping.py
│   │
│   ├── spotify/
│   │   ├── data_cleaning.py
│   │   ├── data_cleaning_2.py
│   │   └── data_extraction.py
│   │
│   ├── wikipedia/
│   │   ├── data_cleaning.py
│   │   └── web_scraping.py
│   │
│   └── merging_and_cleaning/
│       └── final_dataset_merging_and_cleaning.py
│
└── README.md
```

## Detailed Description

### Scripts
- **allmusic**
  - `data_cleaning.py`, `data_cleaning_2.py` – cleaning procedures for AllMusic data  
  - `web_scraping.py` – extraction of raw data from AllMusic  
- **spotify**
  - `data_extraction.py` – data extraction from Spotify  
  - `data_cleaning.py`, `data_cleaning_2.py` – cleaning procedures for Spotify data  
- **wikipedia**
  - `web_scraping.py` – extraction of raw data from Wikipedia  
  - `data_cleaning.py` – cleaning procedures for Wikipedia data  
- **merging_and_cleaning**
  - `final_dataset_merging_and_cleaning.py` – merging of datasets from all sources and final cleaning  

---

### Analysis
- **descriptive_analysis.ipynb** – descriptive statistics as an introduction to exploratory analysis  
- **exploratory_analysis.ipynb** – exploratory analysis applied to the *csny* dataset  

---

### Data
- **AllMusic Datasets**: raw, v2, v3  
- **Spotify Datasets**: raw, v2, v3  
- **Wikipedia Datasets**: raw, v2, v3  
- **combined**  
  - *allmusic-combined*  
  - *wikipedia-combined*  
  - *spotify-combined*  
  - *allmusic-wikipedia-combined*  
- **final**  
  - Dataset created by combining *allmusic-wikipedia-combined* and *spotify-combined*  
  - Includes the *csny* dataset  

---
# How to Run

To reproduce the workflow, follow these steps:

1. **Download the repository folder** to your local machine.
2. **Run the web scraping scripts** for all three data sources:
   - `scripts/spotify/data_extraction.py`
   - `scripts/allmusic/web_scraping.py`
   - `scripts/wikipedia/web_scraping.py`
3. **Run the cleaning scripts** to process the scraped data:
   - `scripts/spotify/data_cleaning.py` and `data_cleaning_2.py`
   - `scripts/allmusic/data_cleaning.py` and `data_cleaning_2.py`
   - `scripts/wikipedia/data_cleaning.py`
4. **Run the final merging and cleaning script** to combine the datasets:
   - `scripts/merging_and_cleaning/final_dataset_merging_and_cleaning.py`
5. **Perform the analysis** using:
   - `analysis/descriptive_analysis.ipynb`
   - `analysis/exploratory_analysis.ipynb`
  

