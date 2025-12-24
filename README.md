# Spotify Trend Analysis

A reproducible exploratory analysis of Spotify tracks and audio features to surface trends in popularity, genres, artists and feature interactions. The analysis is implemented in main.ipynb and uses the provided SpotifyFeatures.csv dataset.

## Project overview

This project explores which audio features and genres influence a track's popularity. The notebook performs data cleaning, feature engineering (e.g., duration in minutes, popularity buckets), and presents visual insights across four main areas:

1. What makes a song popular? (relationship of popularity with danceability, energy, valence, etc.)
2. Genre influence on audio features and popularity.
3. Feature correlations, covariances and interactions (heatmaps / pairplots).
4. Artist & track-level insights (top artists, most popular tracks).

All analysis, plots and code are in main.ipynb.

## Repository structure

- main.ipynb               - Primary Jupyter notebook with the analysis
- SpotifyFeatures.csv      - Dataset used by the notebook (not committed here if large)
- visuals/images/          - Folder for exported visualization images (created)
- README.md                - Project overview (this file)

## How to reproduce the visuals

1. Clone the repository:

   git clone https://github.com/MoinuddinDhorajiwala/Spotify-Trend-Analysis.git
   cd Spotify-Trend-Analysis

2. (Optional but recommended) Create a virtual environment and install dependencies (if you have a requirements.txt):

   python -m venv .venv
   source .venv/bin/activate  # macOS/Linux
   .venv\Scripts\activate     # Windows
   pip install -r requirements.txt

3. Open the notebook and run all cells:

   jupyter notebook main.ipynb

4. Save visualization images from the notebook to visuals/images/.

   In the notebook, after plotting a figure, save it with:

   plt.savefig('visuals/images/<figure_name>.png', dpi=150, bbox_inches='tight')

   Suggested filenames used in this README (examples):
   - visuals/images/danceability_boxplot.png
   - visuals/images/energy_violin.png
   - visuals/images/feature_correlation.png
   - visuals/images/popularity_over_time.png

Once saved, images will display in this README automatically.

## Preview 

![Danceability Across Popularity Buckets](visuals/danceability_across_pop.png)

![Energy Distribution Across Popularity Buckets](visuals/energy_distribution_across_pop.png)

![Danceability Vs Popularity ](visuals/danceability_vs_popularity.png)

![Feature Correlation ](visuals/top5_features_most_correlated.png)

![Feature Covariance ](visuals/top5_most_covariated.png)

![Top 10 Track Count ](visuals/top10_track_count.png)

![Top 10 Most Popular Tracks ](visuals/top10_most_popular_tracks.png)

![Top 10 Genres ](visuals/top10_genres.png)

![Top 10 Artists ](visuals/top10_artist.png)

## Contact

Moinuddin Dhorajiwala — https://github.com/MoinuddinDhorajiwala
