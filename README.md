# 🏖️ Smart Tourism Prediction & Analytics Dashboard  

## Project Overview
This project analyzes global tourism trends by combining **tourist arrivals**, **festival impacts**, **cost of living**, and **tourist reviews** to generate actionable insights. Using **Python and Matplotlib**, it creates a comprehensive **static dashboard** showing:

- Seasonal tourist movement (simulated heatflow)  
- Festival impact vs. tourism intensity  
- Affordability vs. tourism comparison  
- Top 10 countries for strategic tourism campaigns  
- Global tourist sentiment from reviews  

The project is designed for **Framework for Data and Visual Analytics** coursework.  

---

## 📂 Datasets
All datasets used in the project are **synthetic or publicly simulated**:

1. **Tourist Arrivals Dataset**  
   - Years: 1995–2022  
   - Columns: Country, Metric, Yearly Arrivals  

2. **Festival Dataset**  
   - 500 rows  
   - Columns: Festival_Name, Country, Month, Impact_Score, Category, Lat, Lon  

3. **Cost of Living Dataset**  
   - Columns: Country, Cost of Living Index, Rent Index, Groceries Index, Restaurant Price Index, Local Purchasing Power Index  

4. **Travel Reviews Dataset**  
   - Columns: Review, Rating (1–10)  

> Processed versions of all datasets are saved in `data/processed/`.  

---

## 🛠️ Tools & Libraries

- Python 3.x  
- Pandas – data manipulation and cleaning  
- Matplotlib – all static visualizations  
- NumPy – numerical computations
- Plotly – visualization 

> All visualizations are **static for reproducibility**.  

---

## 📖 Project Workflow

### 1️⃣ Notebook 01 – Data Cleaning & Preparation
- Removed duplicates and missing values  
- Normalized numeric metrics  
- Saved processed datasets to `data/processed/`  

### 2️⃣ Notebook 02 – Exploratory Data Analysis & Insights
- Filtered tourist arrivals  
- Aggregated festival impact by country  
- Normalized affordability index  
- Plotted:  
  - Festival Impact vs Tourism Intensity  
  - Affordability vs Tourism Intensity  
  - Top 10 Countries by Combined Score  
  - Global Review Ratings  

### 3️⃣ Notebook 03 – Seasonal Tourist Heatflow
- Simulated seasonal distribution of tourist arrivals  
- Combined festival impact with arrivals to generate **Tourism_Intensity**  
- Created **seasonal bar plots** and simulated **geographical heatflow**  

### 4️⃣ Notebook 04 – Final Combined Dashboard
- Merged all datasets  
- Computed **Combined Score** = Tourism + Festival – Affordability  
- Visualizations included:  
  - Festival vs Tourism  
  - Affordability vs Tourism  
  - Top 10 Countries Combined Score  
  - Global Reviews Histogram  
  - Seasonal Heatflow (simulated)  
- Exported tables for reports (`dashboard_combined.csv`, `top10_countries.csv`)  

---

## 🔍 Key Insights

1. Countries with **high festival impact** tend to attract more tourists.  
2. **Affordability** inversely affects tourism intensity – cheaper countries attract more visitors.  
3. **Top-performing countries** are identified using a combined score of tourism, festival impact, and affordability.  
4. **Tourist reviews** show generally positive sentiment.  
5. Seasonal analysis highlights **peak travel seasons** for planning tourism campaigns.  

---

## Future Work

- Integrate **interactive maps** using Folium or Plotly
- Use **real-time API data** for live tourist predictions
- Incorporate **social media sentiment** for more granular cultural analysis
- Animate **seasonal tourist movement flows** for visual storytelling

---

