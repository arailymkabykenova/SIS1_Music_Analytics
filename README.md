# SIS1_Music_Analytics

Analyzing acoustic features, emotional moods and popularity trends in music (2021-2025).
Course: Data Collection & Preparation, KBTU.

**Team:** Kabykenova Arailym (data collection, scraping, cleaning, merging), Alzhan Fariza (EDA, visualizations, report)

## Data sources
- **Jamendo API** (`/v3.0/tracks/`): 1000 independent tracks released in 2021-2025, with tempo, vocal/instrumental, genres and mood tags.
- **Wikipedia** (web scraping with requests + BeautifulSoup): Billboard Hot 100 number-one singles, 2021-2025.

## Files
| File | Description |
|---|---|
| `SIS_Music_Analytics.ipynb` | Full pipeline: API, scraping, cleaning, merging, EDA, visualizations |
| `report_Music_Analytics.pdf` | Written report |
| `jamendo_tracks.csv` | Raw data from the Jamendo API |
| `billboard_hits.csv` / `billboard_hits_clean.csv` | Scraped Billboard data, raw and cleaned |
| `merged_music.csv` | Final dataset merged by year |
| `plot1.png`, `plot2.png`, `plot3.png` | Visualizations |
| `requirements.txt` | Python libraries |

## How to run
pip install -r requirements.txt
jupyter notebook SIS_Music_Analytics.ipynb

Then run all cells. The Jamendo API sometimes returns an empty page; the notebook retries, and if a page is still missing, run it again.