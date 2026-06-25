# Multi-League Football Analytics Comparison

## Overview
A comparative analytics project analyzing three major European football leagues: Premier League (England), La Liga (Spain), and Bundesliga (Germany). Fetches real-time data from all three leagues using the football-data.org API and performs cross-league analysis to identify competitive trends, scoring patterns, and league rankings.

## Features
- **League Standings**: Top 5 teams from each league (PL, La Liga, Bundesliga)
- **Top Scorers Across All Leagues**: Identifies the best goal scorers globally across all three leagues combined
- **Competitive Gap Analysis**: Compares league competitiveness (points spread between 1st and 5th place teams)
- **Average Goals Per League**: Scoring intensity comparison across the three leagues
- **League Rankings**: Ranks leagues by competitiveness and scoring
- **CSV Exports**: Separate CSV files for each league plus consolidated cross-league results

## Tech Stack
- **Python 3.x**
- **Pandas**: Data manipulation, concatenation, groupby operations, cross-league aggregation
- **NumPy**: Statistical calculations and comparisons
- **Requests**: Multi-league API calls
- **football-data.org API**: Live data from 3 leagues (Premier League, La Liga, Bundesliga)

## How to Run

### Prerequisites
- Python 3.7 or higher
- pip (Python package manager)

### Installation
1. Clone or download this repository
2. Install dependencies:
```bash
   pip install pandas numpy requests
```

### Getting an API Key
1. Go to https://www.football-data.org/client/register
2. Create a free account
3. Copy your API key from the dashboard

### Running the Project
1. Update the script with your API key (replace `YOUR_API_KEY`)
2. Run:
```bash
   python multi_league_analytics.py
```
3. Check output folder for CSV files:
   - `pl_standings.csv`
   - `la_liga_standings.csv`
   - `bundesliga_standings.csv`
   - `top_scorers_all_leagues.csv`
   - `league_comparison.csv`

## Key Insights (Example Results)
- **Top Scorer Across All Leagues**: [Player Name] from [League] with [X] goals
- **Most Competitive League**: [League] (smallest points gap between 1st-5th place)
- **Highest Scoring League**: [League] (avg goals/match)
- **League Ranking by Competition**: 1st: [League], 2nd: [League], 3rd: [League]

## Project Learnings
- Multi-source API integration with parallel data fetching
- Pandas concat() and merge() for combining datasets across different sources
- Cross-dataset analysis and comparative statistics
- Handling large aggregations with nlargest() and groupby()
- Data organization for multi-league analysis projects
- API parameter tuning (season, competition codes)

## Next Steps
- **Computer Vision**: Player and ball tracking using YOLOv8 on match footage
- **Predictive Modeling**: Forecast match outcomes based on league statistics
- **Interactive Dashboard**: Real-time visualization with Flask or Streamlit

## Author
Usama | AI + Sports

## License
MIT
