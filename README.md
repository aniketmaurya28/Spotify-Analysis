# 🎧 Spotify Streaming Analytics Dashboard

## 📊 Dashboard Overview

The dashboard is structured into **four key sections**, accessible via an intuitive navigation menu:

| Page | Description |
|------|-------------|
| 🏠 **Overview** | High-level KPIs and top albums at a glance |
| 🎤 **Artist & Track Insights** | Top artists, tracks, and listening time breakdown |
| 📈 **Listening Trends** | Time-based analysis by year, month, weekday, and hour |
| 📱 **Platform Behaviour** | Platform usage, shuffle/skip rates, and online vs offline listening |

---

## 🔢 Key Metrics (All-Time)

| Metric | Value |
|--------|-------|
| 🎵 Total Track Plays | 26,000+ |
| 🎼 Unique Tracks | 3,012 |
| 💿 Album Titles | 2,461 |
| 🎤 Artist Names | 992 |
| ⏱️ Minutes Played | 80,000+ |
| 🔀 Shuffle Rate | 18.77% |
| ⏭️ Skip Rate | 18.77% |

---

## 🎤 Artist & Track Insights

### Top 10 Played Artists (by Play Count)
1. **Pritam** — 2,767 plays *(Most Played Artist)*
2. Arijit Singh — 946
3. Shankar-Ehsaan-Loy — 721
4. Anuv Jain — 634
5. A.R. Rahman — 618
6. Vishal-Shekhar — 601
7. Rahat Fateh Ali Khan — 578
8. Atif Aslam — 546
9. KK — 395
10. Sachin-Jigar — 372

### Top 10 Played Tracks (by Play Count)
| Track | Plays |
|-------|-------|
| Tu hai kahan | 212 |
| Alag Aasmaan | 196 |
| Husn | 180 |
| Tera Chehra | 189 |
| Mera Mann Kehne… | 180 |
| Pehli Nazar Mein | 150 |
| Baarishein | 146 |
| Saibo | 146 |
| Tere Naina | 137 |
| Teri Jhuki Nazar | 140 |

**Most Played Track:** `Tu hai kahan` | **Most Played Album:** `Rockstar`

---

## 📈 Listening Trends

### Minutes Played by Year
| Year | Minutes | Track Plays |
|------|---------|-------------|
| 2020 | 1K | 0.6K |
| 2021 | 11K | 4.0K |
| 2022 | 12K | 4.0K |
| 2023 | 18K | 5.6K |
| 2024 | 23K *(peak)* | 7.5K *(peak)* |
| 2025 | 13K | 4.0K |
| 2026 | 2K | 0.6K |

### Plays by Day of Week
Thursday leads listening activity (13K plays), followed by Tuesday, Friday, and Monday (12K each). Sunday is the lightest day (9K).

### Peak Listening Hours
The most active listening hours are **12 AM** (3.4K plays) and **11 PM** (3.1K plays), indicating a strong night-time listening pattern.

---

## 📱 Platform Behaviour

### Platform Usage Breakdown
| Platform | Usage Share |
|----------|-------------|
| Android | 85.86% |
| Other | 9.96% |
| Web Player | 2.53% |
| Android TV | 1.65% |
| iOS | 0.01% |

### Listening Mode
- 🟢 **Online:** 91.61%
- ⚫ **Offline:** 8.39%

### Shuffle vs Non-Shuffle
- 🔀 **Shuffle:** 18.77%
- ▶️ **Non-Shuffle:** 81.23%

### Skip Rate by Platform
- Android: **19.6**
- Other: **19.2**

### Minutes Played by Platform
Android dominates with **67K minutes**, followed by Other (9K), Web Player (2K), Android TV (1K), and iOS (0K).

---

## 🗂️ Dataset

The analysis is built on a cleaned Spotify streaming history dataset (`spotify_cleaned_data`) containing **26,255 rows** and **3,012 distinct track values**.

### Key Columns
| Column | Description |
|--------|-------------|
| `platform` | Device/OS used for streaming |
| `Date` & `Time` | Timestamp of each play |
| `Minutes Played` | Duration of each listening session |
| `Track Name` | Name of the track played |
| `Artist Name` | Artist of the track |
| `Album Title` | Album the track belongs to |
| `conn_country` | Connection country (primarily IN) |
| `shuffle` | Whether shuffle mode was active |
| `skipped` | Whether the track was skipped |
| `offline` | Whether played in offline mode |
| `incognito_mode` | Whether private session was active |
| `reason_start` / `reason_end` | How the track started/ended |
| `Platform Clean` | Cleaned/categorised platform label |
| `Week Day` & `Hour of day` | Derived time-based columns |

---

## 🛠️ Tools Used

- **Power BI Desktop** — Data modelling, DAX measures, and interactive visualisations
- **Power Query** — Data cleaning and transformation
- **DAX** — Custom measures (Shuffle Rate, Skip Rate, Online/Offline Rate, etc.)
- **Spotify Extended Streaming History** — Source data exported via Spotify's data request feature

---

## 📁 Repository Structure

```
📦 spotify-dashboard
 ┣ 📂 Dashboard/
 ┃ ┣ 📄 README.md
 ┃ ┣ 🖼️ Spotify Artist & Albums.png
 ┃ ┣ 🖼️ Spotify Listening Trends.png
 ┃ ┣ 🖼️ Spotify Overview.png
 ┃ ┣ 🖼️ Spotify Platform Behaviour.png
 ┃ ┣ 🖼️ Spotify data table_1.png
 ┃ ┗ 🖼️ Spotify data table_2.png
 ┣ 📂 Data/
 ┃ ┣ 📄 README.md
 ┃ ┗ 📊 spotify_cleaned_data.csv
 ┗ 📄 README.md
```

---


> ⚠️ *To use your own data, request your extended streaming history from [Spotify's Privacy page](https://www.spotify.com/account/privacy/) and replace the CSV source.*

---

## 🙋 Author

**Aniket Maurya**

---
