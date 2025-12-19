# 🎵 Spotify Data Analysis & Visualization

## 📌 Project Overview
This project performs exploratory data analysis (EDA) and visualization on large-scale Spotify datasets to uncover trends in music popularity, audio features, song duration, and genre-wise characteristics over time.

The analysis is implemented using Python and focuses on understanding relationships between audio features such as energy, loudness, acousticness, and popularity.

---

## 📂 Datasets Used
### 1. Spotify Tracks Dataset
- ~586,000 tracks
- Features include:
  - popularity, danceability, energy, loudness
  - acousticness, instrumentalness, valence, tempo
  - release_date, duration, artists

### 2. Spotify Features Dataset
- Genre-wise track information
- Used for genre-based popularity and duration analysis

Datasets are sourced from publicly available Spotify datasets on Kaggle.

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 🔍 Analysis Performed

### Data Cleaning & Preprocessing
- Identified missing values (71 missing entries in `name`)
- Converted `release_date` to datetime format
- Set `release_date` as index
- Converted duration from milliseconds to seconds
- Removed non-essential columns for correlation analysis

---

### Popularity Analysis
- Identified least popular songs (popularity = 0)
- Extracted top 10 most popular tracks (popularity > 90)
- Analyzed popularity distribution over time

---

### Correlation & Regression Analysis
- Pearson correlation heatmap of audio features
- Positive correlation observed between **energy and loudness**
- Negative correlation observed between **acousticness and popularity**
- Regression plots for:
  - Loudness vs Energy
  - Acousticness vs Popularity

---

### Time-Based Analysis
- Distribution of number of songs released per year
- Analysis of song duration trends across decades
- Bar plot of average song duration vs year

---

### Genre-Based Analysis
- Comparison of song durations across genres
- Identification of top genres based on popularity
- Genre-wise popularity visualization

---

## 📊 Visualizations
- Correlation heatmap
- Regression plots
- Distribution plots
- Bar plots for time and genre analysis

---

## ▶️ How to Run

### Google Colab (Recommended)
1. Open the notebook in Google Colab
2. Upload or link the datasets
3. Run all cells sequentially

### Local Setup
```bash
pip install pandas numpy matplotlib seaborn
