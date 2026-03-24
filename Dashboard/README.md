## 📈 Dashboard Features 
### Interactive Visualizations
Platform Breakdown: Pie charts showing Android (85%), Web (3%), Others (9%)

- Shuffle vs Non-Shuffle: 81% shuffle usage revealed
- Skip Analysis: 18% overall skip rate by platform
- Temporal Trends: Plays by Year/Month/Day with drill-down
- Top Lists: Artists, Tracks, Albums by minutes & count

## Navigation & UX 
- Multi-page navigation via image buttons
- Drill-through from Year → Month → Day
- Bookmarks for key insights
- Dynamic tooltips & slicers

## 💡 Key Learnings
- DAX Date Formatting: SWITCH(WEEKDAY([Date],2),1,"Monday",2,"Tuesday"...)
- Drill Functionality: Year > Month > Day hierarchical navigation
- Complex Text Processing: Custom Power Query columns for messy categorical data

## 🚧 Challenges Overcome
| Problem                 | Solution                                         |
| ----------------------- | ------------------------------------------------ |
| Messy platform variants | Custom Power Query column with conditional logic |
| Milliseconds to minutes | Pandas column transformation (/ 60000)           |
| Duplicate streams       | df.drop_duplicates()                             |
| Complex skip analysis   | DAX measure with conditional COUNTROWS           |



 🔗 Connect
Aniket Maurya | Final-year BE Computer Engineering
[LinkedIn](https://www.linkedin.com/in/aniket-maurya-68bb4925a/) |  Dashboard PBIX on request!

Skills Demonstrated: Python, Pandas, Power BI, DAX, Power Query, Data Visualization, ETL
