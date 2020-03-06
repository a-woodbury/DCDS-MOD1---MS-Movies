# Novel Movie Studio Analysis
## Flatiron School DC Data Science Module 1 Project
#### Joe Buzzelli and Alphonso Woodbury
Presented 03.06.2020

### Background

Our challenge was to analyze movie industry data and provide a client (Microsoft) guidance for developing a new studio. We provided visuals, analysis, and a brief presentation to share our findings and recommendations. 

#### Questions
To best serve our client, we propose 3 questions after reviewing the available data:
* Which genre(s) are indicated in the highest performing movies over the last five years?
* Is there a relationship between a movies MPAA rating and performance?
* When is the best time to release the film?


#### Data Sources
* The Numbers
* IMDB
* Omdb

#### Assumptions
* Consumer trends evolve rapidly and will only analyze film data since 2015
* Our client will initially focus distribution in the United States


### The data

From the provided datasets, we chose to use the IMDb titles and The Numbers budgets, and added data using the OpenDB API.

The **imdb.titles** and **tn.budgets** datasets were joined on the film titles using a composite id made with the movies year of release; this prevents bad joins on identical films with identical names. 

The **API** data supplemented the provided budget and genre data with MPAA and viewer rating info. The resulting dataset is sorted by domestic profit descending and limited to the top 50 titles released since 2015.

### Findings

* 42% of the Top 50 are Action/adventure

![genrecounts.png](attachment:genrecounts.png)

* Non-Action/Adventure films have higher ROI (on average), but higher budget Action-Adventure films often have higher profit margins

![budgetprofitscatter.png](attachment:budgetprofitscatter.png)

* PG-13 Action/Adventure are the most profitable

![unnamed%20%281%29.png](attachment:unnamed%20%281%29.png)

* Films released in December or June exhibit the highest profits

![unnamed.png](attachment:unnamed.png)

* Action/adventure movies tend to have higher budgets and profits

* PG-13 Action/Adventure are the most profitable

* Films released in December or June exhibit the highest profits

### Recommendations
With a focus on profitability, we recommend that Microsoft produce a film meeting the following criteria:
* Genre: Action/adventure
* MPAA Rating: Rated PG-13
* Release: Released in either December of June.

### Project Expansion Suggestions
* Scope: Test hypothesis against broader data set to explore potential statistical correlations

* Talent: Expand analysis to movie talents’ (directors, writers) impact to profitability

* Voice of the Customer: Conduct sentiment analysis to better understand consumers’ movie interests

