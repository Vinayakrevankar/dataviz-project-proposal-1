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

## NEW ENHANCEMENTS 

This visualization extends the previous bar chart into a stacked bar chart showing how Nobel Prizes are distributed across categories and decades. Each stack represents a time period, and colors indicate different Nobel Prize categories. <br>
### Interactive Features:
Legend Highlighting: Hovering or clicking on a category in the legend isolates that category across all time periods, helping viewers instantly focus on specific trends such as Medicine or Physics.<br>
Color Encoding: Each category is assigned a distinct color for clarity and quick visual comparison.<br>
Smooth Transitions: Bars dynamically adjust when interactions occur, making the visualization feel more fluid and engaging.
### Insights:
Scientific categories like Medicine, Physics, and Chemistry show a clear increase in awards over time.<br>
Peace and Literature remain steady across decades, reflecting slower growth compared to scientific fields.<br>
The stacked structure emphasizes how the overall volume of Nobel Prizes has grown, especially after the 1950s.<br>

https://github.com/user-attachments/assets/157b4fa7-8b7d-4481-b5b0-467065e8fbe7

## Prototype 2:

I created an interactive scatter plot to visualize how songs vary in Energy and Danceability across different genres. Each bubble represents a song, with its color indicating the genre and its size reflecting popularity. The visualization also includes checkbox filters that let users toggle genres on or off, dynamically updating the chart to focus on specific musical styles.

<img width="1360" height="692" alt="image" src="https://github.com/user-attachments/assets/c493c244-9e82-457f-bd43-9063fe5dd0ec" />

VizHub - <a href="https://vizhub.com/Vinayakrevankar/788a38aa88704de795301daf53b07694?file=App.js"> Prototype Link </a>





