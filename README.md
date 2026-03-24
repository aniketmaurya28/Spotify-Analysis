# 🎧 Spotify Streaming Analytics Dashboard

**End-to-End Data Pipeline: Raw Spotify JSON → Interactive Power BI Insights**

Analyzed 15,549 streams spanning 4+ years (46,743 total minutes) to uncover listening patterns, platform preferences, and music tastes through advanced EDA and visualization.

## 📊 Project Overview

Transformed raw Spotify streaming history JSON files into actionable insights using:
- **Python (Pandas/NumPy)**: Data cleaning & EDA
- **Power BI**: Interactive dashboard with custom DAX measures
- **Power Query**: Advanced platform categorization

**Key Metrics Uncovered:**
| Metric | Value |
|--------|-------|
| Total Streams | 26,255 |
| Unique Tracks | 1,883 |
| Unique Albums | 1,501 |
| Unique Artists | 626 |
| Total Minutes | ~ 80K |
| Top Platform | Android (85%) |

## 🛠️ Technical Implementation

### 1. **Data Pipeline**
Raw JSON (8K+9K+9K streams)
↓
Pandas EDA + Cleaning
↓
Clean CSV Export
↓
Power BI Dashboard


### 2. **EDA Operations**
```python
# Key transformations applied
df = pd.read_json('streaming_history.json')
df.drop_duplicates(inplace=True)
df.rename(columns={
    'master_metadata_track_name': 'track_name',
    'master_metadata_album_artist_name': 'artist_name', 
    'ms_played': 'minutes_played'
}, inplace=True)
df['minutes_played'] = df['minutes_played'] / 60000

// Top Artist by Minutes
Top Artist Minutes = 
SUM('SpotifyData'[minutes_played])

// Skip Rate
Skip Rate = 
DIVIDE(
    CALCULATE(COUNTROWS('SpotifyData'), 'SpotifyData'[skipped] = "TRUE"),
    COUNTROWS('SpotifyData')
)
```
🔗 Connect
Aniket Maurya | Final-year BE Computer Engineering
[LinkedIn](https://www.linkedin.com/in/aniket-maurya-68bb4925a/) 

Skills Demonstrated: Python, Pandas, Power BI, DAX, Power Query, Data Visualization, ETL
