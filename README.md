Data Visualization Project

Data

The data I propose to visualize for my project is the Nobel Laureates dataset from Kaggle:
https://www.kaggle.com/datasets/nobelfoundation/nobel-laureates

It contains detailed information on Nobel Prize winners from 1901 to the present, including year, category, laureate demographics, affiliations, and prize share.

---

## Prototype 1:

I’ve created a proof of concept visualization of this data.
It’s a bar chart showing the total number of Nobel laureates by category, using D3.js and a cleaned CSV from the Kaggle dataset.

<img width="1358" height="782" alt="image" src="https://github.com/user-attachments/assets/488302e1-15ad-4eab-ab98-7c51ffbc441b" />

VizHub - https://vizhub.com/Vinayakrevankar/bad3af9c4b7d4ee5a2b63a1add1f3ad2

## NEW ENHANCEMENT 

This visualization extends the previous bar chart into a stacked bar chart showing how Nobel Prizes are distributed across categories and decades. Each stack represents a time period, and colors indicate different Nobel Prize categories.
Interactive Features:
Legend Highlighting: Hovering or clicking on a category in the legend isolates that category across all time periods, helping viewers instantly focus on specific trends such as Medicine or Physics.
Color Encoding: Each category is assigned a distinct color for clarity and quick visual comparison.
Smooth Transitions: Bars dynamically adjust when interactions occur, making the visualization feel more fluid and engaging.
Insights:
Scientific categories like Medicine, Physics, and Chemistry show a clear increase in awards over time.
Peace and Literature remain steady across decades, reflecting slower growth compared to scientific fields.
The stacked structure emphasizes how the overall volume of Nobel Prizes has grown, especially after the 1950s.

https://github.com/user-attachments/assets/157b4fa7-8b7d-4481-b5b0-467065e8fbe7



