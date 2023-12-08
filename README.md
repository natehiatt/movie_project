![ReadMe header](images/readme_header.png)
# Movie Industry Data Analysis
## Overview
Our firm is advising a company that plans to venture into the movie industry by setting up a new movie studio. Our clients require that we use available data to explore what films have done well and why. They have tasked us with finding trends and relationships in this data that may guide their decisions. Such exploration may include recommendations on movie type, who to hire, when to make movies, how much to spend, etc., all in order to maximize profits. By the end of our analysis, we will provide five data-backed and statistically tested recommendations for our client's new movie studio.

The data we will use is publicly available through [IMDB](https://www.imdb.com/), [Box Office Mojo](https://www.boxofficemojo.com/), [Rotten Tomatoes](https://www.rottentomatoes.com/), [The Movie Database (TMDB)](https://www.themoviedb.org/), and [The Numbers](https://www.the-numbers.com/).

Our presentation can be found here: [Slide Deck](https://docs.google.com/presentation/d/1RR23O4ka1Zdvgp1HC9cLXy5smHbgusWzRsVdYAl3bDw/edit?usp=sharing) 

## Business Understanding
The movie industry is dominated by large, established studios. The "Big Five" include Universal, Paramount, Warner Bros., Disney, and Sony. These companies have the connections, influence, and deep pockets to create most of the well-known blockbusters we see in theaters today. However, their tactic of mass appeal leaves portions of the market open for smaller studios. 

Audiences are extremely diverse, with many movie-goers preferring lower budget, more niche storytelling. Smaller studios like A24 became extremely successful off of complex, high-quality films made with lesser-known actors.


## Data Understanding

The IMDB database contains 150k records, and from it we took information on directors, writers, movie runtime, and release dates.

The Numbers dataset consists of about 6k records, and we use it for its financial information: domestic gross and production budget. While the size of this dataset is a small fraction of the other two, it is also our most extensive source of financial data, which is a crucial metric of success.

Finally, the Movie Database (TMDB) consists of about 27k records. Its most important metric is the popularity rating, which is calculated as a "lifetime" score. It takes into account viewer votes and views, watchlisting, and total number of votes. The breakdown for what is included can be found here: [TMDB Popularity Score](https://developer.themoviedb.org/docs/popularity-and-trending). 

Every dataset contained information on movie title, so we were able to connect our datasets using title. 

## Data Preparation
3 independent variables
major code
: outliers and which data sets were joined

## Analysis and Results/Recommendations
iMPLICATIONS FOR STAKEHOLDERS, their real-world problem, goal
1. timing
2. 3D
3. creators
4. budget
5. runtime

## Limitations of Data
While we have access to production budget for the movies in our data, there are other aspects of budget, such as marketing budget, that would have changed our ROI calculations.

Our sample of 3-D movies was ultimately cut down to just 10 movies, which diminishes our ability to find a statistically significant result and the overall value of this analysis. This is 

## Potential Next Steps
We were able to provide five actionable insights to our clients using only certain parts of three of the datasets available. In the future, we encourage further exploration of all available data. For example, researchers might look at the profit potentials of hiring certain actors over others, of distributing movies in certain countries, of different genres of movies, etc.

Although not in the scope of this project, building a predictive model based on the strength of relationships between various production variables could provide more insights about how a planned production may perform.

## Repo Structure
```
├── data
│   ├── tn.movie_budgets.csv.gz
│   ├── tmdb.movies.csv.gz
│   ├── rt.reviews.tsv.gz
│   ├── imdb.db.zip
│   ├── bom.movie_gross.csv.gz
├── Images
├── Notebooks
│   ├── data_cleaning.ipynb
│   ├── data_cleaning-jay.ipynb
│   ├── scratch_graphs.ipynb
│   ├── __pycache__
│   ├── nate_scratch.ipynb
│   ├── shelley_scratch.ipynb
│   ├── jay_scratch.ipynb
├── .gitignore
├── Final.ipynb
├── LICENSE
├── README.md
```
