![splash.jpg](https://github.com/a-woodbury/Greenlight/blob/master/Resources/greenlightsplash.png)

**Novel Movie Studio Analysis**


### Overview

Our challenge was to analyze movie industry data and provide a client (Microsoft) guidance for developing a new studio. We provided visuals, analysis, and a brief presentation to share our findings and recommendations. 

* Which genre(s) are indicated in the highest performing movies over the last five years?
* Is there a relationship between a movies MPAA rating and performance?
* When is the best time to release the film?

### Repository Navigation
<pre>
Technical Notebook : <a href=https://github.com/a-woodbury/Greenlight/blob/master/notebooks/mod1_jbaw_analysis%26viz_aw.ipynb>Technical Notebook </a>
Dataset Links      : <a href=https://github.com/a-woodbury/Greenlight/tree/master/data>Data</a>
Presentation       : <a href=https://github.com/a-woodbury/Greenlight/blob/master/Presentation/Mod1%20Project%20Presentation%20v2.pptx.pdf>Slide Deck</a>
</pre>

### ReadME Navigation

[Problem](https://github.com/a-woodbury/Greenlight/blob/master/README.md#problem) - 
[Data](https://github.com/a-woodbury/Greenlight#data) -
[Results](https://github.com/a-woodbury/Greenlight#results) - 
[Recommendations](https://github.com/a-woodbury/Greenlight#recommendations) - 
[Future](https://github.com/a-woodbury/Greenlight#future) - 
[Project Info](https://github.com/a-woodbury/Greenlight#project-info) -

## Problem

**Assumptions:**
* Consumer trends evolve rapidly and will only analyze film data since 2015
* Our client will initially focus distribution in the United States


## Data 
* The Numbers
* IMDB
* Omdb




### The data

From the provided datasets, we chose to use the IMDb titles and The Numbers budgets, and added data using the OpenDB API.

The **imdb.titles** and **tn.budgets** datasets were joined on the film titles using a composite id made with the movies year of release; this prevents bad joins on identical films with identical names. 

The **API** data supplemented the provided budget and genre data with MPAA and viewer rating info. The resulting dataset is sorted by domestic profit descending and limited to the top 50 titles released since 2015.

## Results

* 42% of the Top 50 are Action/adventure

![genrecounts.png](https://github.com/a-woodbury/Greenlight/blob/master/images/genrecounts.png)

* Non-Action/Adventure films have higher ROI (on average), but higher budget Action-Adventure films often have higher profit margins

![budgetprofitscatter.png](https://github.com/a-woodbury/Greenlight/blob/master/images/budgetprofitscatter.png)

* PG-13 Action/Adventure are the most profitable

![unnamed%20%281%29.png](https://github.com/a-woodbury/Greenlight/blob/master/images/Screen%20Shot%202020-03-05%20at%2012.55.06%20PM.png)

* Films released in December or June exhibit the highest profits

* Action/adventure movies tend to have higher budgets and profits

* PG-13 Action/Adventure are the most profitable

* Films released in December or June exhibit the highest profits

### Recommendations
With a focus on profitability, we recommend that Microsoft produce a film meeting the following criteria:
* Genre: Action/adventure
* MPAA Rating: Rated PG-13
* Release: Released in either December of June.

## Future
* Scope: Test hypothesis against broader data set to explore potential statistical correlations

* Talent: Expand analysis to movie talents’ (directors, writers) impact to profitability

* Voice of the Customer: Conduct sentiment analysis to better understand consumers’ movie interests


## Project Info

<pre>
Contributors : <a href=https://github.com/a-woodbury>Alphonso Woodbury</a>
               <a href=https://github.com/a-woodbury>Joe Buzzelli</a>
</pre>

<pre>
Languages    : Python
Tools/IDE    : Anaconda
Libraries    : 
</pre>

<pre>
Duration     : March 2020
Last Update  : 06.05.2020
</pre>

<pre>
Domain       : 
Sub-Domain   : 
Techniques   :  
Application  : 
</pre>
