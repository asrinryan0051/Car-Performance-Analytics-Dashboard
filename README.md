# Car Performance Analytics Dashboard

## Project Overview
This project is an interactive, client-side dashboard designed to provide granular analysis of key performance metrics for a dataset of **34 popular vehicles in the Indian automobile market**.

The core objective is to showcase proficiency in the data science pipeline:  
**from raw data ingestion and feature engineering to delivering advanced, interactive visualizations**, all within a **portable, zero-dependency web environment**.

---

## 🚀 Unique Value Proposition: Large-Scale Analysis

### Why this dashboard exists:
Most popular Indian automotive websites restrict users to comparing only **2 or 3 cars at a time**.  
This makes it impossible to see where a vehicle stands in the context of the **entire market**.

### This dashboard solves that problem by enabling:

#### ✔ Macro-Level Comparison  
Visualize **34+ vehicles simultaneously** to identify segment leaders and outliers instantly.

#### ✔ Dynamic Filtering  
Users can drill down into specific **Brands** or **Fuel Types** to analyze sub-segments.  
Example:  
> *"Show me performance stats for all Diesel SUVs."*

---

## 📊 Core Visualizations & Insights

The application uses **four distinct visualization methods** to provide a comprehensive view of performance.  
Here is how to interpret them:

---

### 1. **BHP vs. Acceleration (Scatter Plot)**
**Visualization Type:** Scatter Plot  
**Application & Insight:**  
- Shows the relationship between **raw power (BHP)** and **Acceleration (0–100 km/h time)**  
- Helps identify which car offers the **best blend of high power and quick acceleration**  
- Users should look for dots in the **top-left** or **bottom-right**, depending on axis orientation  
- Useful for finding the **performance sweet spot**

---

### 2. **Average BHP by Brand (Bar Chart)**
**Visualization Type:** Bar Chart  
**Application & Insight:**  
- Provides a macro-level understanding of **manufacturer performance philosophy**  
- By averaging BHP across each brand’s lineup, users can identify:  
  - **Performance-focused brands**  
  - **Commuter/economy-focused brands**

---

### 3. **Top Speed Distribution (Box Plot)**
**Visualization Type:** Box Plot  
**Application & Insight:**  
- Shows the statistical distribution of **top speeds** across **different fuel types**  
- Users can immediately see:  
  - Minimum top speed  
  - Maximum top speed  
  - Median and interquartile ranges  
- Works best when using global filters to isolate **specific fuel types**

---

### 4. **Engine Ratio vs. Speed (Line Plot)**
**Visualization Type:** Line Plot  
**Application & Insight:**  
A key visualization that analyzes the **BHP-to-Torque Ratio**, a crucial engineering parameter.

- **High Ratio:**  
  Indicates a **rev-happy engine** that builds power at high RPM  
  - Typically found in sporty petrol engines  

- **Low Ratio:**  
  Indicates strong **low-end pulling power**  
  - Typical of torquey diesel engines  

This helps users understand deeper engine characteristics beyond just BHP and torque values.

---

## 📑 Important Note on Data Selection

To ensure a fair performance comparison, specific **engine variants** were selected for each car model in the dataset.

### Methodology:
- When a car model has **multiple engine options**, the variant with the **highest BHP** is always selected.  
- This ensures that no car is unfairly underrepresented in the comparison.

### Example:
- **Hyundai Creta**  
  - Comes in both Petrol and Diesel  
  - Petrol variant chosen because it generates **higher horsepower**  

### Future Updates:
A later version of this project will include **all available engine options** for every model.

---

## 🛠️ Technology Stack & Architecture

This project is built using only **native web technologies**, ensuring maximum portability and reliability.

| Technology | Role | Reason for Use |
|-----------|------|----------------|
| **HTML5 & Vanilla CSS** | Structure and Styling | Lightweight layout, avoids heavy frameworks like Tailwind, ensures fast load times even offline |
| **JavaScript (ES6+)** | Data Cleaning & Logic | Performs filtering, grouping, aggregation, and feature generation directly in the browser (similar to Pandas) |
| **Plotly.js** | Visualization Engine | Renders professional interactive charts (Scatter, Bar, Box, Line) |
| **GitHub Pages** | Deployment | Allows hosting as a fully static, single-file dashboard |

---

## ⚙️ Dashboard Features

### 1. **Smart Cascading Filters**
The filter controls are **interconnected** and dynamically adapt to the dataset.

- Selecting a **Brand** (e.g., Mahindra) automatically removes unavailable fuel options (e.g., Hybrid).  
- Selecting a **Fuel Type** (e.g., Diesel) updates the Brand list to show only those manufacturers that offer Diesel vehicles in the dataset.

This ensures users never encounter **empty visualizations** or invalid filter combinations.

---

### 2. **🌙 Dedicated Dark Mode (Built-In)**
The dashboard includes a **fully integrated Dark Mode toggle**, allowing users to switch between:

- **Light Mode:** Clean, bright, and traditional analytical layout  
- **Dark Mode:** High-contrast, eye-comfort design suitable for long analysis sessions  

Dark Mode also includes:  
- Dark-themed Plotly charts  
- Auto-adjusting backgrounds  
- Theme-preserving dropdowns and filter controls  
- Smooth transitions without page reloads  

---

## ▶️ How to Run the Project Locally

This project is designed for **instant execution** with **zero installation**.

### Steps:
1. **Download the File**  
   Copy the content of the `index.html` file and save it locally as **index.html**

2. **Open in Browser**  
   Double-click the saved file  
   The dashboard will load and execute all data processing and charting automatically

No Python, no Node.js, no server required.

---
## ⚠️ Disclaimer

This project is created for **educational and portfolio purposes only**.  
All car brand names, models, and specifications belong to their respective owners.  
This project is **not affiliated with or endorsed by any car manufacturer**.

---



