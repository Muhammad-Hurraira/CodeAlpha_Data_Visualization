# Netflix Data Analysis Project

## 📋 Project Overview
Analysis of Netflix's content library to understand content distribution, genre popularity, and platform strategy.

## 📊 Dataset Analysis
**File**: `Netflix.csv`  
**Size**: 7,787 entries, 12 columns  
**Key Features**: Content type, title, director, cast, country, date_added, release_year, rating, duration, genres

### 🔍 Data Quality Assessment
**Missing Values Identified**:
- Director: 2,389 missing (30.7%)
- Cast: 718 missing (9.2%) 
- Country: 507 missing (6.5%)
- Date_added: 10 missing (0.1%)
- Rating: 7 missing (0.09%)

## ✅ Completed Analyses

### 1. Data Preprocessing
**Cleaning Operations**:
- Filled missing director/cast/country with 'Unknown'
- Removed rows with missing date_added
- Filled missing ratings with mode (most frequent)
- Converted dates: "14-Aug-20" → datetime format
- Extracted features: year_added, month_added

**Result**: Clean dataset with 7,777 rows, 14 columns, no missing values

### 2. Content Type Distribution
**Visualization**: Pie chart  
**Finding**:
- **Movies**: 69.7% of library
- **TV Shows**: 30.3% of library

**Insight**: Netflix's content strategy heavily favors movies over TV series

### 3. Top 10 Genre Analysis
**Method**: Extracted individual genres from comma-separated strings  
**Top Genres**:
1. International Movies - 2,652 titles
2. Dramas - 2,426 titles  
3. Comedies - 1,590 titles
4. Action & Adventure - 1,397 titles
5. International TV Shows - 1,300 titles
6. Documentaries - 869 titles
7. Romantic Movies - 766 titles
8. Thrillers - 742 titles
9. Kids' TV - 671 titles
10. TV Dramas - 661 titles

**Visualization**: Horizontal bar chart with Netflix styling  
**Key Insight**: International content dominates, showing Netflix's global strategy

## 🎨 Technical Implementation
**Tools Used**: Python, Pandas, Matplotlib, Seaborn, Jupyter  
**Styling**: Netflix brand colors (#E50914 red, #221F1F black)  
**Code Features**:
- Flexible date parsing with `format='mixed'`
- Professional visualizations with proper labeling
- Progressive analysis approach

## 📈 Key Business Insights
1. **Content Imbalance**: 70/30 split favoring movies suggests strategic focus on film content
2. **International Dominance**: Top genre being "International Movies" aligns with global expansion
3. **Genre Concentration**: Top 3 genres account for significant library portion
4. **Data Collection Gaps**: ~30% missing director data indicates metadata improvement opportunities

## 🔄 Project Structure
```
Netflix_Analysis/
├── Netflix_Data_Visualization.ipynb  # Main notebook
├── NetFlix.csv                       # Dataset
├── README.md                         # Documentation
└── requirements.txt                  # Dependencies
```

## ⚙️ Setup Instructions
```bash
# Install dependencies
pip install pandas matplotlib seaborn jupyter

# Run analysis
jupyter notebook Netflix_Data_Visualization.ipynb
```

## 📌 Requirements
```txt
pandas>=1.3.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
```

## ⏳ Project Status
**Completed**: Data cleaning, basic distribution analysis, genre ranking  
**Not Implemented**: Temporal trends, rating distributions, geographic analysis, duration patterns, summary insights  
**Completion**: ~40% of planned analyses

## 💡 Future Work
Planned but not implemented analyses:
- Content additions over time
- Rating comparisons between Movies/TV Shows
- Top content-producing countries
- Movie runtime vs TV show season analysis
- Cross-genre and cross-country relationships

## 📬 Contact

For any queries or feedback, feel free to connect!
- LinkedIn: https://www.linkedin.com/in/muhammad-hurraira-0993a4346/

## 📝 Note
Educational project using publicly available Netflix data. Analysis shows foundational insights but requires completion of planned sections for comprehensive understanding.

## 🎯 Quick Findings
- Movies are Netflix's primary content type (69.7%)
- International Movies is the most common genre category
- Data quality issues exist, particularly with director information
- Netflix shows strong international content focus
- Top genres indicate strategic content investments in dramas and comedies

---

**Purpose**: Educational Data Analysis
