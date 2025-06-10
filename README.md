# FIFA 23 Player Dataset: Exploratory Data Analysis (EDA)

![FIFA 23 Logo](https://upload.wikimedia.org/wikipedia/en/thumb/d/d1/FIFA_23_cover_art.jpg/320px-FIFA_23_cover_art.jpg)

Comprehensive EDA of FIFA 23 player attributes to uncover insights about player performance, valuation, and career trajectories.

## 📌 Project Overview
This project analyzes 17,000+ FIFA 23 players through:
- Statistical profiling
- Positional attribute comparisons
- Age-performance relationships
- Talent clustering
- Geospatial talent distribution

Key questions answered:
- What physical/skill attributes differentiate positions?
- When do players typically peak in their careers?
- Which countries produce the highest-rated players?
- How are player attributes correlated?

## 🛠️ Tech Stack
- **Python 3** (Pandas, NumPy)
- **Visualization**: Matplotlib, Seaborn, Plotly
- **Geospatial**: Plotly Express
- **Statistical Analysis**: SciPy, scikit-learn

## 📂 Dataset
**Source**: [FIFA 23 Complete Player Dataset](https://www.kaggle.com/datasets/kevwesophia/fifa23-official-datasetclean-data) (Kaggle)  
**Original Columns**: 89  
**Cleaned Columns**: 25 after processing  
**Key Attributes**:
- Player demographics (Age, Nationality, Position)
- Performance metrics (Overall, Potential)
- Physical attributes (Height, Weight)
- Contract details

## 🔍 EDA Highlights

### 1. Positional Attribute Profiles
![Radar Chart](images/position_radar.png)  
*Goalkeepers show distinct physical traits compared to outfield players*

### 2. Age-Performance Relationship
![Age vs Potential](images/age_potential.png)  
*Peak potential occurs at age 24 for most positions*

### 3. Global Talent Distribution
![World Map](images/nationality_map.png)  
*Traditional football nations dominate player production*

### 4. Player Clustering
![PCA Clusters](images/pca_clusters.png)  
*Clear separation between elite players and role players*

## 🧹 Data Cleaning Steps
1. Removed visual columns (photos, flags)
2. Standardized currency values (£110M → 110,000,000)
3. Converted heights (5'11" → 180cm) and weights (154lbs → 70kg)
4. Handled missing data:
   - Filled missing `Body Type` with mode
   - Marked missing `Loaned From` as "Not on Loan"
5. Created new features:
   - `Years_at_Club`
   - `Value_per_Wage_Ratio`

## 📊 Key Findings
1. **Positional Differences**:
   - Strikers have highest skill moves (avg 3.2/5)
   - Center-backs are tallest (avg 188cm)
2. **Career Peaks**:
   - Outfield players peak at 24-28 years
   - Goalkeepers peak later (27-31 years)
3. **Talent Hotspots**:
   - Brazil produces highest avg rated players (67.2)
   - England has most players (1,422)

