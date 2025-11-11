# 🌳 NYC Trees & Heat
---
**Author:** Meghan Kret   
**Class:** Data Visualization - Midterm Part 2  
**Due Date:** November 11 2025   

---
## Overview
This project explores how the presence of street trees relates to neighborhood heat vulnerability across New York City. It visualizes the connection between canopy cover and climate risk using live NYC Open Data. Built as a scroll-based D3.js experience, the piece invites users to explore patterns of heat, shade, and equity across the five boroughs.

---

## Theme Connection
Aligned with the DxD 2026 theme **“Ecosystems and Cycles of Life,”** this project treats the city as a living ecosystem. Trees are part of the cycle of growth and renewal that helps regulate heat and sustain urban life. The visualization shows how the absence or abundance of trees reflects broader social and environmental systems. IE, how the city breathes, grows, and struggles against climate stress.

---

## Live Demo
👉 **View the project here:**  
[https://meghanrn.github.io/NYC-Trees-and-Heat/](https://meghanrn.github.io/NYC-Trees-and-Heat/)  

---

## 📊 Datasets
- **Heat Vulnerability Index (HVI)** — NYC Department of Health and Mental Hygiene  
  [https://data.cityofnewyork.us/resource/4mhf-duep.json](https://data.cityofnewyork.us/resource/4mhf-duep.json)

- **2015 Street Tree Census** — NYC Department of Parks & Recreation  
  [https://data.cityofnewyork.us/resource/uvpi-gqnh.json](https://data.cityofnewyork.us/resource/uvpi-gqnh.json)

- **MODZCTA Boundaries** — NYC Open Data  
  [https://data.cityofnewyork.us/api/geospatial/pri4-ifjk?method=export&format=GeoJSON](https://data.cityofnewyork.us/api/geospatial/pri4-ifjk?method=export&format=GeoJSON)

### Data Notes
- Filtered to valid ZIP areas and living trees only.  
- Aggregated by ZIP to compute tree density (trees per km²).  
- Outliers winsorized to reduce skew.  
- HVI matched to tree data using shared MODZCTA codes.  

### Bias & Limitations
- Tree data from 2015 (outdated and excludes private or park trees).  
- HVI compresses multiple factors into a single score (simplified).  
- No population weighting, so area-based comparison may misrepresent exposure.  
- Data collected by city agencies may contain geographic or reporting bias.

---

## Features
- Scroll-based storytelling flow that guides the viewer through multiple scenes  
- Dual map view: compare Heat Vulnerability vs. Tree Density  
- Hover and tooltip interactions for detailed values  
- Scatter plot showing the relationship between trees and heat  
- Highlighted outlier neighborhoods that defy the general trend  
- Bivariate equity map highlighting high-HVI/low-tree areas  
- Fully client-side — no backend or build tools required  

---

## Reflection
> The NYC Trees & Heat project demonstrates how data visualization can make environmental inequity visible. What works well is how the scrolling story and interactive maps let users connect data with place. They can literally see how areas with more trees tend to have lower heat vulnerability. The live NYC Open Data connection keeps the project grounded in real, public information. What doesn’t work as well yet is the uneven quality of the data: the tree census is from 2015, and it only includes street trees, not those in parks or private yards. Also, some high-vulnerability areas don’t fit the trend, showing that factors like housing quality and air conditioning access are equally important. Next, I’d like to add population weighting and accessibility features like better keyboard navigation. Overall, the project fits the “Ecosystems and Cycles of Life” theme by showing how urban ecosystems (made up of both people and trees) shape cycles of heat, shade, and resilience across the city.

---

## Tech
- **Language:** HTML
- **Library:** D3.js (v7)  
- **Hosting:** GitHub Pages  
- **Data Source:** Live from NYC Open Data APIs  

---

## Instructions
1. Clone or download this repository.  
2. Open `index.html` in your browser, or visit the GitHub Pages link above.  
3. Scroll through the story, hover on neighborhoods, and drag the map divider to explore differences.
