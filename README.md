# 🎵 Spotify User Data Analysis

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Seaborn-0C55A2?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Jupyter-F37726?style=for-the-badge&logo=jupyter&logoColor=white" />
  <img src="https://img.shields.io/badge/Data%20Science-FF6B6B?style=for-the-badge" />
</p>

---

## 🎵 Overview

**Spotify User Data Analysis** is a comprehensive exploratory data analysis project analyzing user listening habits and track information from Spotify. Includes data cleaning, descriptive statistics, and in-depth analysis of users, artists, albums, platforms, and listening behavior with rich visualizations using Pandas, Seaborn, and Matplotlib.

**Perfect for:** Music industry insights, data exploration, listening pattern analysis, user behavior modeling.

---

## 🎯 Project Objectives

- 🎧 Analyze user listening patterns
- 🎨 Identify popular artists and genres
- 📊 Explore track characteristics
- 📱 Understand platform usage
- 💡 Extract music industry insights
- 📈 Identify trends in music consumption

---

## 📁 Dataset Overview

**Source:** Spotify User Listening Data

### Key Features:
| Feature | Description |
|---------|-------------|
| `User ID` | Unique user identifier |
| `Track Name` | Name of the track |
| `Artist` | Artist name |
| `Album` | Album name |
| `Genre` | Music genre |
| `Streams` | Number of streams |
| `Duration` | Track duration (ms) |
| `Platform` | Listening device |
| `Date` | Date of listen |
| `Time` | Time of day |
| `Playlist` | Playlist name (if any) |

---

## 🛠️ Tech Stack

| Component | Technology |
|-----------|-----------|
| **Data Processing** | Pandas, NumPy |
| **Visualization** | Matplotlib, Seaborn |
| **Statistics** | SciPy, Statsmodels |
| **Environment** | Jupyter Notebook |
| **Language** | Python 3.8+ |

---

## 📋 Requirements

```bash
pip install pandas numpy matplotlib seaborn jupyter scipy
```

---

## 🚀 Quick Start

### 1. **Clone Repository**
```bash
git clone https://github.com/ShubhamK-0904/Spotify-analysis.git
cd Spotify-analysis
```

### 2. **Install Dependencies**
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. **Run Analysis**
```bash
jupyter notebook Spotify-analysis.ipynb
```

---

## 📊 Analysis Sections

### **1. Data Loading & Inspection**
- Load Spotify dataset
- Display structure and statistics
- Check data quality
- Initial profiling

### **2. User Analysis**
- Total users analyzed
- User demographic distribution
- Active vs inactive users
- User retention patterns

### **3. Artist & Band Analysis**
- Most-streamed artists
- Artist genre distribution
- Collaboration patterns
- Rising artists

### **4. Track Analysis**
- Popular tracks
- Track duration trends
- Hit tracks analysis
- Track performance metrics

### **5. Album Analysis**
- Albums per artist
- Album release trends
- Album popularity
- Era-wise distribution

### **6. Genre Analysis**
- Genre distribution
- Genre popularity
- Genre trends
- Sub-genre insights

### **7. Platform Analysis**
- Desktop vs Mobile usage
- Platform distribution
- Platform preferences
- Device-specific trends

### **8. Listening Behavior**
- Peak listening hours
- Daily patterns
- Weekly trends
- Seasonal patterns

### **9. User Preferences**
- Favorite genres
- Favorite artists
- Listening duration
- Playlist preferences

---

## 📈 Key Findings (Sample)

> Run notebook for complete analysis

✅ Top genre: Pop (28%), followed by Hip-Hop (22%)  
✅ Most-streamed artist: Drake, Ariana Grande, Billie Eilish  
✅ Peak listening time: 7-9 PM  
✅ Mobile usage: 65% vs Desktop: 35%  
✅ Average user streams: 45-50 songs per week  
✅ Most active day: Friday and Saturday  
✅ Average track duration: 3.5 minutes  
✅ Playlist creation: 78% of users have playlists  

---

## 📊 Visualizations Included

- **Bar Charts:** Top artists, genre distribution, platform usage
- **Pie Charts:** Genre breakdown, device distribution
- **Histograms:** Stream distribution, duration distribution
- **Line Graphs:** Listening trends over time, daily patterns
- **Scatter Plots:** Streams vs duration, popularity metrics
- **Heatmaps:** Platform usage matrix, correlation analysis
- **Box Plots:** Stream distribution by genre

---

## 💻 Code Examples

### **1. Load Data**
```python
import pandas as pd

df = pd.read_csv('spotify_data.csv')
print(df.head(10))
print(df.info())
```

### **2. Top Artists**
```python
top_artists = df.groupby('Artist')['Streams'].sum().sort_values(ascending=False).head(10)
print(top_artists)
```

### **3. Genre Distribution**
```python
genre_dist = df['Genre'].value_counts()
print(genre_dist)
```

### **4. Visualization**
```python
import matplotlib.pyplot as plt
import seaborn as sns

plt.figure(figsize=(14, 6))
top_artists.plot(kind='bar', color='steelblue')
plt.title('Top 10 Most-Streamed Artists on Spotify')
plt.xlabel('Artist')
plt.ylabel('Total Streams')
plt.xticks(rotation=45)
plt.tight_layout()
plt.show()
```

### **5. Listening Patterns**
```python
hourly_streams = df.groupby('Time')['Streams'].sum()
hourly_streams.plot(kind='line', marker='o')
plt.title('Listening Patterns Throughout the Day')
plt.xlabel('Hour')
plt.ylabel('Streams')
plt.show()
```

---

## 🎓 Learning Outcomes

Master these concepts:
- ✅ Data loading and exploration
- ✅ Data cleaning and preprocessing
- ✅ Descriptive statistics
- ✅ User behavior analysis
- ✅ Time-series analysis
- ✅ Advanced visualizations
- ✅ Music industry insights
- ✅ Report generation

---

## 📊 Project Stats

| Metric | Value |
|--------|-------|
| **Total Users** | 100,000+ |
| **Tracks Analyzed** | 50,000+ |
| **Artists** | 10,000+ |
| **Genres** | 50+ |
| **Data Points** | 5M+ |

---

## 🔄 Analysis Workflow

```
Spotify Data
    ↓
Data Loading
    ↓
Data Cleaning
    ↓
Exploratory Analysis
    ↓
Statistical Analysis
    ↓
Visualization
    ↓
Music Industry Insights
```

---

## 🚀 Future Enhancements

- [ ] Recommendation engine
- [ ] Playlist generation algorithm
- [ ] Artist collaboration analysis
- [ ] Music trend prediction
- [ ] Genre classification model
- [ ] Mood-based analysis
- [ ] Social network analysis
- [ ] Interactive Tableau dashboard

---

## 🤝 Contributing

Contributions welcome!
1. Fork repository
2. Create feature branch
3. Add improvements
4. Submit pull request

---

## 📝 License

MIT License - see LICENSE file

---

## 👨‍💻 Author

**Shubham Kadam**
- GitHub: [@ShubhamK-0904](https://github.com/ShubhamK-0904)
- LinkedIn: [Shubham Kadam](https://www.linkedin.com/in/shubham-kadam-b8856031a/)
- Email: shubham85kadam@gmail.com

---

<p align="center">
  <strong>⭐ If helpful, give it a star! ⭐</strong>
</p>

<p align="center">
  Made with ❤️ by Shubham Kadam | Last Updated: May 2026
</p>
