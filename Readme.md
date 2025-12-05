# Nobel Prize Data Visualization Project - Final Report

This project presents a series of interactive visualizations exploring more than a century of Nobel Prize awards. Using **D3.js**, I transformed the Nobel dataset into a set of visual stories that highlight trends across categories, countries, laureates, and time. The project began with simple prototypes and gradually expanded into richer, multi-view, highly interactive visualizations.

The goal was not just to display data, but to help users explore it-zooming into specific categories, comparing countries, isolating patterns over decades, and tracking how different award areas have changed over time.

---

## 1. Dataset Overview

**Dataset:** The Nobel Prize Dataset (Kaggle)  
**Coverage:** 1901–2024  

**Fields include:**
- Prize category  
- Year  
- Laureate name  
- Country  
- Prize share  
- Motivation text  
- Gender  
- Organization / affiliation  

This dataset is ideal for visualization because it combines categorical, temporal, geographic, and hierarchical data.

---

## 2. Project Goals

This project focuses on answering key questions such as:

- Which countries have produced the most Nobel laureates?  
- How have prize categories grown or changed over time?  
- Which categories dominate different decades?  
- How do scientific categories compare to Peace and Literature?  
- What long-term global patterns are visible?

To explore these questions, I created multiple visualization prototypes, each adding new interaction techniques and visual encodings.

---

## 3. Prototype Visualizations

### Prototype 1 - Bar Chart: Nobel Prizes by Category

This chart ranks countries by total number of Nobel Prizes.

**Why this visualization works**

Bar charts are ideal for comparing categorical data. Sorting the bars makes rankings immediately understandable.

**Features**
- Hover tooltip with exact counts  
- Mouseover highlighting  
- Bars sorted descending by award totals  

**Insights**
- The United States and United Kingdom dominate prize counts.  
- Western Europe shows dense representation.  
- There is a long tail of countries with only 1–3 laureates.

<img width="1358" height="782" alt="image" src="https://github.com/user-attachments/assets/488302e1-15ad-4eab-ab98-7c51ffbc441b" />

VizHub - https://vizhub.com/Vinayakrevankar/bad3af9c4b7d4ee5a2b63a1add1f3ad2

---

### Prototype 2 - Line Chart: Awards Over Time (By Category)

This line chart shows yearly award totals for a selected category.

**Interactions**
- Category dropdown selector  
- Hover tooltips displaying year and count  
- Dot markers for individual data points  

**Insights**
- Physics has strong early activity and remains steady.  
- Peace prizes skip several years.  
- Scientific fields show steep growth after mid-century.

<img width="1228" height="732" alt="image" src="https://github.com/user-attachments/assets/1e6d7d19-3f0e-4574-a2ab-218a2f5e80c7" />

VizHub - https://vizhub.com/Vinayakrevankar/13061a401abe428f8f7328391c57204b

---

## 4. New Enhancement - Stacked Bar Chart: Category Distribution by Decade

**(Fully implemented - major project enhancement)**

This visualization extends the bar chart concept into a stacked bar chart showing category totals per decade.

**Encoding**
- Each bar = one decade  
- Each stack segment = one category  

**Interactive Features**
- **Legend Highlighting:** Clicking or hovering isolates that category across all decades.  
- **Smooth Transitions:** Animations for fading, resizing, and re-stacking.  
- **Color Encoding:** Unique colors assigned to each category.

**Insights**
- Physics, Chemistry, and Medicine increase significantly after the 1950s.  
- Peace and Literature remain comparatively stable.  
- Stacking clarifies overall growth trends over time.

VizHub - <a href="https://vizhub.com/Vinayakrevankar/9c343639e1464ab99a791dc46bf618e6"> Prototype Link </a>

https://github.com/user-attachments/assets/157b4fa7-8b7d-4481-b5b0-467065e8fbe7


---

## 5. Prototype 3 - Choropleth Map: Geographic Distribution

This visualization maps Nobel Prize distribution by country.

**Features**
- Country coloring based on award totals  
- Hover tooltip with numeric details  
- Gradient legend scale

**Insights**
- North America and Western Europe dominate.  
- Asian representation rises in modern decades.  
- Very limited representation across Africa.

<img width="964" height="540" alt="image" src="https://github.com/user-attachments/assets/51e8b6d0-9c58-4315-a092-f2bf2a78a6fb" />

VizHub - https://vizhub.com/Vinayakrevankar/dfa78c8e0bc843c4a74429d82a474142

---

## 6. Prototype 4 - Treemap: Category–Laureate Structure

This treemap explores hierarchical relationships between prize categories and individual laureates.

**Features**
- Hierarchical layout  
- Rectangle size encodes number of prizes  
- Category-based color grouping  
- Detailed hover tooltips

**Insights**
- Scientific categories produce the largest laureate groupings.  
- Peace prizes appear more evenly distributed across recipients.

<img width="964" height="556" alt="image" src="https://github.com/user-attachments/assets/e69654d3-7b00-47f0-bffc-e690c29f9f0d" />


VizHub - https://vizhub.com/Vinayakrevankar/53e394cc97c9490487ca9535e4bdad09

---

## 7. Prototype 5 - Ring Chart: Category Share

A donut-style ring chart illustrating the proportional distribution of Nobel categories.

**Insights**
- Scientific awards dominate total prize volume.  
- Peace and Literature account for consistently smaller shares.

_Insert ring chart screenshot here_

---

## 8. Final Integrated Dashboard

The final stage unified all prototypes into a single interactive dashboard.

**Dashboard Features**
- Dataset overview and summary statistics  
- Category distribution by decade (stacked bars)  
- Award trends by category (line chart)  
- Nobel country leaderboard (bar chart)  
- Laureate treemap and category ring chart  
- Interactive elements: sliders, dropdowns, brushing, highlights, transitions

This integrated design creates a connected exploratory environment where users can transition seamlessly between trends, geographic patterns, categorical breakdowns, and high-level summaries.

<img width="2984" height="5438" alt="image" src="https://github.com/user-attachments/assets/16d833b2-992d-4957-a079-a97643f88a5b" />

VizHub - https://vinayakrevankar.com/data-visualization/

---

## Conclusion

This project demonstrates how layered interactive visualizations can transform raw historical data into meaningful stories. The dashboard enables users to investigate how Nobel Prizes evolve over time, across geographic regions, and among categories-supporting both high-level overview analysis and focused, detail-driven exploration.
