# Movie Database Capstone Project README

## Project Overview
This notebook explores a dataset of TV shows available on various streaming platforms (Netflix, Hulu, Prime Video, Disney+). The project aims to analyze ratings, distribution across streaming services, and correlations between different metrics to gain insights into the TV show landscape.

## Key Findings

### General Rating Insights
*   **IMDb Ratings:** Ranged from 1.0 to 9.6.
*   **Rotten Tomatoes Ratings:** Ranged from 6.0 to 100.0.
*   **Average Rating Comparison:** When scaled to a 0-10 range, Rotten Tomatoes ratings (average ~7.75) were slightly higher on average than IMDb ratings (average ~7.11).

### Streaming Service Distribution
*   **Total Shows (Raw Data):** Prime Video hosts the most shows (2144), followed by Netflix (1931), Hulu (1754), and Disney+ (180).
*   **Overlap:** A few shows, such as "Lab Rats" and "Jessie", are available on both Netflix and Disney+.

### Cleaned Dataset Analysis
*   **Dataset Size:** After removing rows with missing values, the cleaned dataset (`df_nona`) contains 931 TV shows.
*   **Age Group Distribution:** The '16+' age group contains the highest number of TV shows in the cleaned dataset.
*   **Rating Distributions (Histograms):** Visual analysis of histograms showed a general trend of higher ratings for both IMDb and Rotten Tomatoes, with IMDb having a more concentrated peak at higher values.
*   **Streaming Service Distribution (Cleaned Data):** In the cleaned dataset, Prime Video still leads with the most shows, followed by Netflix, Hulu, and Disney+.
*   **Top Show Identification:** Rotten Tomatoes ratings (0-100 scale) were deemed potentially more useful for differentiating top shows due to their wider range.
*   **Top IMDb Shows (2011+ with 100% RT):** No TV shows from the top 10 IMDb rated shows (released in 2011 or later) achieved a perfect 100% Rotten Tomatoes score.
*   **Top-Rated 16+ Show (IMDb):** "Sherlock" was identified as the top-rated TV show in the '16+' age bracket based on IMDb ratings.
*   **Network Presence for Top 100 IMDb Shows:** Out of the top 100 IMDb-rated shows (from the cleaned dataset), Netflix had 46, Hulu had 42, Prime Video had 29, and Disney+ had 5. This indicates a strong presence of top-rated shows on Netflix and Hulu.

### Correlations
*   **Most Positively Correlated:** IMDb ratings and Rotten Tomatoes ratings showed the strongest positive correlation (~0.48).
*   **Most Negatively Correlated:** Netflix and Hulu streaming service indicators showed the strongest negative correlation (~-0.56), suggesting an inverse relationship in content availability between these two platforms.
