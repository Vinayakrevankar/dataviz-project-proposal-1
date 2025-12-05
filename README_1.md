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

VizHub - <a href="https://vizhub.com/Vinayakrevankar/9c343639e1464ab99a791dc46bf618e6"> Prototype Link </a>

https://github.com/user-attachments/assets/157b4fa7-8b7d-4481-b5b0-467065e8fbe7

## Prototype 2:

I created an interactive scatter plot to visualize how songs vary in Energy and Danceability across different genres. Each bubble represents a song, with its color indicating the genre and its size reflecting popularity. The visualization also includes checkbox filters that let users toggle genres on or off, dynamically updating the chart to focus on specific musical styles.

<img width="1360" height="692" alt="image" src="https://github.com/user-attachments/assets/c493c244-9e82-457f-bd43-9063fe5dd0ec" />

VizHub - <a href="https://vizhub.com/Vinayakrevankar/788a38aa88704de795301daf53b07694?file=App.js"> Prototype Link </a>


## Week 11
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

