# 🎢 Roller Coaster EDA

This project performs **Exploratory Data Analysis (EDA)** on a dataset of roller coasters from around the world.  
The goal is to clean the data, explore trends, and visualize interesting patterns in coaster design and performance.

---

## 📂 Dataset

The dataset (`coaster.csv`) contains information about over 1,000 roller coasters, including:

- **Coaster_Name** – name of the roller coaster  
- **Location** – where it is located  
- **Status** – whether it’s operating, closed, or under construction  
- **Manufacturer** – company that built the coaster  
- **Year_Introduced** – year the coaster opened  
- **Type** – construction type (wood, steel, launched, etc.)  
- **Speed_mph** – maximum speed  
- **Height_ft** – maximum height  
- **Inversions** – number of upside-down elements  
- **Gforce** – maximum G-force experienced  

---

## ⚙️ Project Workflow

### 1. Data Cleaning
- Dropped irrelevant columns (`Opening date`)  
- Renamed columns for consistency  
- Converted dates into proper datetime format  
- Checked and handled missing values  
- Removed duplicates based on coaster name, location, and opening date  

### 2. Data Exploration
- Counted missing values with `df.isna().sum()`  
- Checked for duplicate coaster entries  
- Queried specific coasters (e.g., *Crystal Beach Cyclone*)  

### 3. Visualizations
- **Top 10 years** with the most coaster introductions (bar chart)  
- **Distribution of speeds** (histogram & KDE plot)  
- **Speed vs Height** comparison (scatter plot, colored by year introduced)  
- **Correlation analysis** of numeric features (heatmap)  

---

## 📊 Key Insights
- Certain years saw **large spikes** in coaster introductions.  
- Most coasters fall within a **moderate speed range**, with few extreme outliers.  
- **Taller coasters generally tend to be faster**, as shown in the scatter plot.  
- Correlation analysis shows relationships between **height, speed, inversions, and G-force**.  

---

## 🛠️ Tech Stack
- **Python** (Pandas, NumPy) – data wrangling  
- **Matplotlib & Seaborn** – data visualization  

---

## 🚀 How to Run
1. Clone the repository or download the project files.  
2. Install dependencies:  
   ```bash
   pip install pandas numpy matplotlib seaborn
