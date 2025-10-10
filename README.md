Solution 1 — README.md 

Data Visualization Project

Data

The data I propose to visualize for my project is the Nobel Laureates dataset from Kaggle:
https://www.kaggle.com/datasets/nobelfoundation/nobel-laureates

It contains detailed information on Nobel Prize winners from 1901 to the present, including year, category, laureate demographics, affiliations, and prize share.


---

Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:

How many Nobel Prizes have been awarded across different categories?

How does the distribution of prizes by category change over time?

Are there noticeable differences in gender or nationality among laureates?

Which organizations and countries have the most affiliated Nobel winners?



---

Sketches

Sketch 1: Nobel Prizes Distribution by Category

A bar chart where the x-axis is the category (Physics, Chemistry, Medicine, Literature, Peace, Economics) and the y-axis is the number of laureates.

Future Interaction ideas: hover to see counts and percentages, filter by decade or gender in future versions.

This directly answers: “How many Nobel Prizes have been awarded across different categories?”

---
Sketch 2: Nobel Prizes Awarded Over Time

A line chart where the x-axis is time (by decade) and the y-axis is the number of Nobel Prizes awarded. Each line represents a prize category.

Future Interaction ideas:
Filter by specific category (e.g., Physics only, or Peace only).
Highlight key historical periods such as the World Wars or the addition of the Economics prize in 1969.


---

Prototypes 1:

I’ve created a proof of concept visualization of this data.
It’s a bar chart showing the total number of Nobel laureates by category, using D3.js and a cleaned CSV from the Kaggle dataset.

<img width="1358" height="782" alt="image" src="https://github.com/user-attachments/assets/488302e1-15ad-4eab-ab98-7c51ffbc441b" />

VizHub - https://vizhub.com/Vinayakrevankar/bad3af9c4b7d4ee5a2b63a1add1f3ad2

---

Prototype 2 - Line Chart (Nobel Prizes per Decade by Category)
I created a line chart showing the number of Nobel Prizes awarded per decade, broken down by category (Medicine, Physics, Chemistry, Literature, Peace, Economics).
This visualization highlights how Nobel Prizes have changed over time:
Medicine, Physics, and Chemistry dominate throughout the 20th century.
Economics appears only after 1969, when the prize was first established.
Peace and Literature remain consistently smaller in number compared to the science prizes.
Peaks and dips align with historical contexts — for example, global wars and social movements.
This prototype extends beyond the static category totals from the bar chart and begins to capture temporal patterns, which is crucial for understanding the evolution of Nobel Prizes.

<img width="1228" height="732" alt="image" src="https://github.com/user-attachments/assets/1e6d7d19-3f0e-4574-a2ab-218a2f5e80c7" />

VizHub - https://vizhub.com/Vinayakrevankar/13061a401abe428f8f7328391c57204b

---

Prototype 2 - Updated Based on Feedback
Add checkbox so that we can filter what is required on viz
<img width="964" height="540" alt="image" src="https://github.com/user-attachments/assets/ac51a637-5cd1-4ff5-88cd-4304898c6457" />


https://vizhub.com/Vinayakrevankar/d662cff112534331abc0c852b3910070

---

Prototype 3 -  Nobel Prizes by Country (Choropleth Map)
This sketch represents a world map visualization where each country is shaded based on the number of Nobel Prizes associated with it — either through birth country or organization affiliation.
Purpose:
To reveal the geographical concentration of Nobel laureates and highlight how recognition varies across regions.
Planned Insights:
Identify the most represented countries (e.g., United States, UK, Germany, France).
Compare the dominance of Western nations versus emerging contributors.
Provide a global context to complement the previous category and timeline analyses.

Future Interaction Ideas: <br>
Hover tooltips showing country names and prize counts.<br>
Toggle between birth country and organization country views.<br>
Click on a country to filter the timeline or category charts dynamically.<br>


<img width="964" height="540" alt="image" src="https://github.com/user-attachments/assets/51e8b6d0-9c58-4315-a092-f2bf2a78a6fb" />

---

Prototype 4 - Nobel Laureates by Category and Country (Treemap Visualization)

This sketch represents a Treemap that visualizes the hierarchical distribution of Nobel Prizes by category and birth country (or organization).
Each rectangle’s size corresponds to the number of laureates, and the color can indicate either prize category or region.
Purpose:
To explore the relative contribution of each country within different Nobel categories and to visually compare the scale of achievements across categories and geographies.
Planned Insights:
Quickly identify which categories dominate globally (e.g., Medicine and Physics).
See which countries contribute most within each category.
Highlight how Nobel Prizes are distributed not just overall, but hierarchically — from category → country.

Future Interaction Ideas:<br>
Hover tooltips showing category, country, and laureate count.<br>
Click to zoom into a single category or region.<br>

<img width="964" height="556" alt="image" src="https://github.com/user-attachments/assets/e69654d3-7b00-47f0-bffc-e690c29f9f0d" />


VizHub - https://vizhub.com/Vinayakrevankar/6582b154c0b54ce4a5ca8a039b31e788

--- 

Prototype 5 -

<img width="1260" height="724" alt="image" src="https://github.com/user-attachments/assets/fae25d03-3287-44bf-9587-fb8cf601391c" />


---

Open Questions

Should I normalize counts by decade to avoid the growth over time dominating the view?

Do I need to separate individuals from organizations in the counts?

How should I handle shared prizes (1/2, 1/3, 1/4 shares) — count as one laureate each, or weight by share?



---

Milestones

Week 1: Basic bar chart of laureates by category (✅ current prototype)

Week 2: Add filters for decade and gender

Week 3: Add map of laureate birth countries and organizational affiliations

Week 4: Finalize dashboard with interactivity and polish.
