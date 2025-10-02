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

Interaction ideas: hover to see counts and percentages, filter by decade or gender in future versions.

This directly answers: “How many Nobel Prizes have been awarded across different categories?”





---

Prototypes 1:

I’ve created a proof of concept visualization of this data.
It’s a bar chart showing the total number of Nobel laureates by category, using D3.js and a cleaned CSV from the Kaggle dataset.

<img width="1358" height="782" alt="image" src="https://github.com/user-attachments/assets/488302e1-15ad-4eab-ab98-7c51ffbc441b" />



Prototype 2

Line Chart (Nobel Prizes per Decade by Category)
I created a line chart showing the number of Nobel Prizes awarded per decade, broken down by category (Medicine, Physics, Chemistry, Literature, Peace, Economics).
This visualization highlights how Nobel Prizes have changed over time:
Medicine, Physics, and Chemistry dominate throughout the 20th century.
Economics appears only after 1969, when the prize was first established.
Peace and Literature remain consistently smaller in number compared to the science prizes.
Peaks and dips align with historical contexts — for example, global wars and social movements.
This prototype extends beyond the static category totals from the bar chart and begins to capture temporal patterns, which is crucial for understanding the evolution of Nobel Prizes.

<img width="1642" height="970" alt="image" src="https://github.com/user-attachments/assets/fec9104b-00bb-4b07-a396-fe1cdb5d687c" />



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
