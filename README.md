# Final-Project-Tableau
---
## Project/Goals
This project aims to analyze Causes of Death statistics from the **The Global Burden of Disease** study to identify trends, outliers, 
and insights to understand our world better. 

## Process
1. Data connection to clean [Kaggle](https://www.kaggle.com/datasets/ivanchvez/causes-of-death-our-world-in-data?resource=download) dataset version.
2. Detected and validated data types for analysis via Tableau built-in data interpreter.
3. Explored dataset by creating 5 preliminary visualizations, and replaced and refined them as my questions became clearer.
4. Realized the 'death numbers' measured lacked normalization to population of a country, resulting in skewed data.
5. Located [World Bank](https://data.worldbank.org/) dataset via Google search to add population data to make sense of the death numbers relative to a country's population.
6. Used understanding from exploratory visualization in order to formulate questions to lead to meaningful insights.
7. Created a dashboard to present findings from Disease/Population statistics.

## Results - Option 2

### Datasource:
> https://www.kaggle.com/datasets/ivanchvez/causes-of-death-our-world-in-data/data

### Questions

The overarching questions as I explored the dataset changed. Here are the overall ones that were the most meaningful.

- What causes of death are prevalent in different areas of the world?
- How do death numbers change over time and what could this look like in the coming years ahead?
- Are there any countries with disproportionately large deaths per capita? Speculate as to why this could be?


### Visualizations & Why

1. Deaths by Causes - *Horizontal Bar Chart*
This quickly showed me a high level overview of the distribution of deaths across different causes so I could quickly explore this new dataset.
However, this visualization will be quickly replaced by a more meaningful bar chart.
2. Most Deaths by Numbers - *Packed bubbles *
This quickly shows me the few dominating causes as represented by the size of the bubbles.
This visualization isn't the best as due to the number of different factors (33) there aren't enough colors in a palette to use this visualization effectively.
3. Map of Deaths Across Nations - *Temperature Map* 
This quick and simple geographical map conveys the potential hot spots for mortality rates by Death Numbers.
> This helped me come to the conclusion that the results may be skewed as certain countries with larger populations will of course have higher mortality rates for all causes. Thus, I will need to add population data to paint a more accurate picture.

4. Top Causes by Death Numbers - *Bar graph* (*revisited 1. bar chart but filtered to Rank the top 10*)
This visualization quickly ranks the top 10 death numbers. This will be used within my dashboard. When a user selects a country they will be able to quickly see the top features which lead to death.
5. Time series Death by Years - *Continuous line graph*
See basic slope and direction of the deaths over time. This graph will be replaced with a more meaningful one.
6. Outliers - *Death causes and countries box plots*
These box plots quickly tell us in a visually accessible way that Cardiovascular diseases and neoplasms are disproportionately impactful compared to all other causes. As well, China and India are much farther outside the whiskers. 
This confirms that I should bring in population data to account for these populous nations.
7. Deaths per Capita - *Map*
This revised map quickly shows us the nations in the dataset, larger circle marks tell us which countries have a higher death rate proportionate to their population.
8. Diseases over Time - *Line graph*
This graph quickly shows us how causes over time(year 1990 - 2019) change. On the right there is a 'causes' box where users can filter by factor. From this graph you can begin to ask questions such
as which diseases increased or decreased and what may have impacted this.
9. Forecasting Disease by Country - *Line graph prediction*
This graph tells us the trend prediction for the next couple years. Users are able to filter by Country as well as Cause name. The predictive continuation line is easily visible in red.

## Challenges & Lessons Learnt

| Challenge   |      Lesson |
|:----------|:-------------|
| Indecisive about direction to go in  | Improve Research practices, speak to peers/mentors sooner |
| Time constraints | Create Minimum Viable Product sooner than later     |
| Skewed data    | Added population metric |
| Data Cleaning   | Address anomolies identified, i.e. United States vs America naming convention  |
| Data Wrangling   | Data ingested from World Bank had years as field name, which required pivot. Used Excel feature but learnt it could be done more efficiently within Tableau itself  |
| Interpreting journal specific data | Google search i.e. neoplasm |


## Future Goals

I would clean the dataset myself. Both as a learning exercise as well and as 'due diligence' so I can trust and make decisions on what to clean etc.
However, in the interest of time, it makes sense to focus on Tableau capabilities to quickly gain insights and visualize them.
I may want to group countries by continent/regions, by bringing in a new dataset, to explore how the region affects the disease distribution. There are many other metrics from World Bank, that can be explored such as education, and economic status.