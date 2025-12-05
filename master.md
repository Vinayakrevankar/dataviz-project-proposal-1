Data Visualization Project


Dataset Overview

Dataset: The Nobel Prize Dataset (Kaggle)
Coverage: 1901–2024
Fields Include:
Prize category
Year
Laureate name
Country
Prize share
Motivation text
Gender
Organization / affiliation
This dataset is ideal for visualization because it mixes categorical, temporal, geographic, and hierarchical data.

2. Project Goals
The project focuses on answering questions such as:
Which countries have produced the most Nobel laureates?
How have prize categories grown or changed over time?
Which categories dominate different decades?
How do scientific categories compare to peace and literature?
What long-term global patterns are visible?
To answer these, I created a series of prototypes, each introducing different interactions and encoding techniques.


---

Prototype 1: Bar Chart: Nobel Prizes by Category
I created a simple proof-of-concept visualization showing the total number of Nobel laureates in each major prize category. This bar chart provides a quick overview of how awards are distributed across fields such as Medicine, Physics, Chemistry, Peace, Literature, and Economics. The data was loaded from a cleaned CSV derived from the Kaggle Nobel Laureates dataset and rendered using D3.js.
This visualization establishes a baseline understanding of the dataset and helps highlight which categories dominate historically. Medicine, Physics, and Chemistry have the highest counts, while Literature, Peace, and Economics show comparatively fewer awards.

<img width="1358" height="782" alt="image" src="https://github.com/user-attachments/assets/488302e1-15ad-4eab-ab98-7c51ffbc441b" />

VizHub - https://vizhub.com/Vinayakrevankar/bad3af9c4b7d4ee5a2b63a1add1f3ad2

---
Prototype 2: Line Chart (Nobel Prizes per Decade by Category)
I created a line chart showing Nobel Prizes awarded per decade, broken down by category (Medicine, Physics, Chemistry, Literature, Peace, Economics).
This visualization highlights:
Medicine, Physics, and Chemistry dominate throughout the 20th century.
Economics appears only after 1969.
Peace and Literature remain consistently smaller in number.
Peaks and dips align with historical events.

<img width="1228" height="732" alt="image" src="https://github.com/user-attachments/assets/1e6d7d19-3f0e-4574-a2ab-218a2f5e80c7" />

VizHub - https://vizhub.com/Vinayakrevankar/13061a401abe428f8f7328391c57204b

---

Prototype 2.1: Based on Feedback I have added checkboxes to allow users to filter and display only the required data on the graph. This enhancement improves interactivity and makes it easier to focus on specific datasets or parameters as needed.

<img width="964" height="540" alt="image" src="https://github.com/user-attachments/assets/ac51a637-5cd1-4ff5-88cd-4304898c6457" />

VizHub - https://vizhub.com/Vinayakrevankar/d662cff112534331abc0c852b3910070

---

Prototype 3: Choropleth Map – Nobel Prizes Won by Country
I created a choropleth map showing the global distribution of Nobel Prizes by country, based on the laureate’s birth country or affiliated organization.
Each country is shaded according to the number of prizes associated with it — darker shades indicate more laureates.
This visualization helps reveal geographic trends in Nobel achievements:
The United States, United Kingdom, Germany, and France appear as major hubs for Nobel winners.
Countries in Europe and North America dominate the upper ranges, while most regions in Africa and parts of Asia have lighter shades, indicating fewer laureates.
The map uses an intuitive color gradient and legend for clear interpretation.
This phase shifts the project focus from purely categorical or temporal analysis to spatial understanding, showing how Nobel recognition is distributed around the world.

<img width="964" height="540" alt="image" src="https://github.com/user-attachments/assets/51e8b6d0-9c58-4315-a092-f2bf2a78a6fb" />

VizHub - https://vizhub.com/Vinayakrevankar/dfa78c8e0bc843c4a74429d82a474142

---

Prototype 4: Treemap – Hierarchical Distribution of Nobel Prizes
I created a Treemap visualizing Nobel Prizes hierarchically by category and country, where each block’s size reflects the number of laureates.
This visualization builds on the previous map by shifting from geographical location to hierarchical relationships, making it easier to see which countries lead within each prize category.
Key Observations:
Medicine, Physics, and Chemistry form the largest sections, confirming their dominance in Nobel history.
Within each category, United States, United Kingdom, and Germany occupy the most significant areas.
Smaller but consistent contributors such as France, Sweden, and Japan appear across multiple categories, highlighting long-term participation.
Design Notes:
Implemented in D3.js, aggregating laureates by (category, birth_country).
Each rectangle is color-coded by category for visual separation.
Tooltips display the country, category, and total laureates when hovered.

<img width="964" height="556" alt="image" src="https://github.com/user-attachments/assets/e69654d3-7b00-47f0-bffc-e690c29f9f0d" />

VizHub - https://vizhub.com/Vinayakrevankar/53e394cc97c9490487ca9535e4bdad09

--- 

Prototype 5: Spotify Genre Popularity Heatmap (2010–2019)
I created a Heatmap visualization displaying average song popularity by genre and year from 2010 to 2019 using D3.js.
Each cell’s color corresponds to the mean popularity score of songs within that genre for a given year.
Key Observations:
Pop, Dance Pop, and Hip Hop maintain consistent high popularity throughout the decade.
A surge in EDM, Tropical House, and Alternative R&B is visible between 2013–2017, reflecting global electronic trends.
Some niche genres like Baroque Pop or Irish Singer-Songwriter appear sporadically, suggesting momentary regional or viral influence.
Popularity diversification increased post-2015, showing more evenly distributed interest across genres.
Design Notes:
Implemented in D3.js with a color scale from light (low popularity) to dark (high popularity).
Dataset sourced from Spotify API / Kaggle data.
Each rectangle represents the mean popularity value of a genre-year pair.
The color legend provides intuitive reference for trend strength.

<img width="1260" height="724" alt="image" src="https://github.com/user-attachments/assets/fae25d03-3287-44bf-9587-fb8cf601391c" />

VizHub - https://vizhub.com/Vinayakrevankar/6582b154c0b54ce4a5ca8a039b31e788

---

Prototype 6: 

I created an interactive scatter plot to visualize how songs vary in Energy and Danceability across different genres. Each bubble represents a song, with its color indicating the genre and its size reflecting popularity. The visualization also includes checkbox filters that let users toggle genres on or off, dynamically updating the chart to focus on specific musical styles.

<img width="1360" height="692" alt="image" src="https://github.com/user-attachments/assets/c493c244-9e82-457f-bd43-9063fe5dd0ec" />

VizHub - <a href="https://vizhub.com/Vinayakrevankar/788a38aa88704de795301daf53b07694?file=App.js"> Prototype Link </a>

---

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

VizHub - <a href="https://vizhub.com/Vinayakrevankar/9c343639e1464ab99a791dc46bf618e6"> Prototype Link </a>

https://github.com/user-attachments/assets/157b4fa7-8b7d-4481-b5b0-467065e8fbe7

## Prototype 6:

I created an interactive scatter plot to visualize how songs vary in Energy and Danceability across different genres. Each bubble represents a song, with its color indicating the genre and its size reflecting popularity. The visualization also includes checkbox filters that let users toggle genres on or off, dynamically updating the chart to focus on specific musical styles.

<img width="1360" height="692" alt="image" src="https://github.com/user-attachments/assets/c493c244-9e82-457f-bd43-9063fe5dd0ec" />

VizHub - <a href="https://vizhub.com/Vinayakrevankar/788a38aa88704de795301daf53b07694?file=App.js"> Prototype Link </a>


## Dashboard
This week, I explored a new dataset: The Oscar Awards Dataset from Kaggle.
It contains detailed historical information on Academy Award nominations and wins, including films, nominees, award categories, and award years.
The dashboard visualizes different facets of Oscar history using multiple linked, interactive views.

1.⁠ ⁠Dataset Information Panel
A brief summary layout describing the dataset, including:
What the dataset represents
Time span of Oscar ceremonies
High-level metadata (films, people, categories, etc.)
Notes on award types such as major categories, technical categories, and honorary awards
This section gives users context before interacting with the visualizations.

2.⁠ ⁠Key Stats Panel
A high-level overview highlighting:
Total award entries
Range of years in the dataset
Total categories
Film and nominee coverage
Designed as a quick snapshot to help users understand the scale of the dataset.

3.⁠ ⁠Category Distribution by Decade (Stacked Bar Chart)
A stacked bar chart showing how Oscar nominations are distributed across categories for each decade.
What it shows
Trends in award volumes across decades
Growth in new categories (e.g., VFX, Sound Editing, Animated Film)
Stability of core acting categories
Interactions
Start Decade Slider – chooses the beginning decade range
End Decade Slider – chooses the ending decade
The stacked chart updates dynamically to show only the selected decade window
Color legend identifies each award category clearly
Insights
Rapid increase in total nominations after the 1970s
Explosion of technical categories in modern decades
Acting, directing, and writing remain consistent across decades

4.⁠ ⁠Award Trends Over Years (Category Trend Line)
A single-category trend line showing how many nominations a specific category receives each year.
Interactions
Category Dropdown – switch between categories (e.g., Best Picture, Actor in a Leading Role)
Line updates instantly to show year-by-year variation
Insights
Some categories show early spikes (e.g., acting awards in the 1930s)
Technical categories appear only in later decades
Categories like “Best Picture” stabilize over time

5.⁠ ⁠Film–Category Network Graph (Force-Directed Network)
A force-directed graph showing connections between top-award-winning films and the categories they won.
Nodes
Blue Nodes → Films
Green Nodes → Award Categories
Interactions
Top Films Slider – choose how many of the most awarded films to display (e.g., Top 10, Top 20)
Draggable Nodes – users can drag films or categories to explore clusters
Hover tooltips show film titles or category names
Insights
Films like Titanic, Gone with the Wind, and Ben-Hur form strong clusters
Highly awarded films connect to multiple technical and major categories
Rare clusters appear for discontinued categories

6.⁠ ⁠Top Award Winners (Horizontal Bar Chart)
A ranked bar chart of the top individuals or studios by number of Oscars won.
Interactions
Top N Slider – adjust how many top winners to display
Bars dynamically resize
Tooltip shows exact award count
Insights
Walt Disney remains the all-time award leader
Major studios like Metro-Goldwyn-Mayer also dominate early years
Some countries (e.g., Italy, France) appear due to honorary or foreign film categories

7.⁠ ⁠Category-Film Treemap (Hierarchical Layout)
A hierarchical treemap where:
Each block represents a category
The nested blocks represent films within that category
Block size corresponds to number of nominations
What It Reveals
Categories with the largest number of films involved
Films that dominate particular award areas
Overall structure of Oscar nominations by type

8.⁠ ⁠Class–Category–Film Sunburst (Radial Hierarchy)
A three-level sunburst showing:
Outer Ring → Films
Middle Ring → Award Categories
Inner Ring → General Class (Acting, Directing, Technical, etc.)
Interactions
Hover tooltips highlight path (Class → Category → Film)
Radii adjust based on nomination/win counts
Insights
Acting and Technical classes have the largest share
Visual Effects and Sound categories grow significantly after the 1970s
Easy to see category diversity within each class

9.⁠ ⁠Category Share Pie Chart
A simple pie chart showing overall share of nominations by category.
Interactions
Hover to show percentage + raw counts
Color-coded to match other charts
Insights
Most nominations cluster in acting categories
Sound and technical awards make up a large portion of modern Oscars
  
10.⁠ ⁠Films Per Decade (Bar Chart)
Shows how many films received nominations or wins in each decade.
Insights
Dramatic growth after 1970s
Spike in decades with industry expansion (e.g., 1990s–2010s) 
Early decades have fewer films due to smaller industry scale

<img width="2984" height="5438" alt="image" src="https://github.com/user-attachments/assets/16d833b2-992d-4957-a079-a97643f88a5b" />

VizHub - <a href="https://vinayakrevankar.com/data-visualization/"> Prototype Link </a> 

How should I handle shared prizes (1/2, 1/3, 1/4 shares) — count as one laureate each, or weight by share?


