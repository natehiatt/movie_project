![ReadMe header](images/readme_header.png)
# Movie Industry Data Analysis
## Overview
Our firm is advising a company that plans to venture into the movie industry by setting up a new movie studio. Our clients require that we use available data to explore what films have done well and why. They have tasked us with finding trends and relationships in this data that may guide their decisions. Such exploration may include recommendations on movie type, who to hire, when to make movies, how much to spend, etc., all in order to maximize profits. By the end of our analysis, we will provide five data-backed and statistically tested recommendations for our client's new movie studio.

The data we will use is publicly available through [IMDB](https://www.imdb.com/), [Box Office Mojo](https://www.boxofficemojo.com/), [Rotten Tomatoes](https://www.rottentomatoes.com/), [The Movie Database (TMDB)](https://www.themoviedb.org/), and [The Numbers](https://www.the-numbers.com/).

In addition, our presentation can be found here: [Slide Deck](https://docs.google.com/presentation/d/1RR23O4ka1Zdvgp1HC9cLXy5smHbgusWzRsVdYAl3bDw/edit?usp=sharing) 

## Business Understanding
The movie industry is dominated by large, established studios. The "Big Five" include Universal, Paramount, Warner Bros., Disney, and Sony. These companies have the connections, influence, and deep pockets to create most of the well-known blockbusters we see in theaters today. However, the

STAKEHOLDERS: could use the project and how

## Data Understanding
source and properties of the data, why it's useful
size of dataset
which features are included
limitations of data

## Data Preparation
3 independent variables
major code
: outliers and which data sets were joined

## Analysis and Results/Recommendations
iMPLICATIONS FOR STAKEHOLDERS, their real-world problem, goal

### Analysis: Release Month

Below, we graphically explore the relationship between the month of release of a movie and, first, the average domestic gross revenue, and second, the average domestic ROI.

![Gross Revenue v. ROI](images/grossVmonth.png)

![ROI v. Month](images/roiVmonth.png)

From these graphs, there are a few main takeaways:

First, the month in which you release a film matters. We can see summer is indeed the time for blockbusters -- May through July has the highest domestic gross numbers, and some of the highest domestic ROI. We can also see a bump in gross revenue at the end of the year. This, presumably, reflects the run-up to the Oscars, when studios release some of the movies that they think are most likely to garner them prestigious awards. Notably, however, **the ROI for those same months is much lower.** This would be explained by the fact that large studios are willing to swallow losses -- that they are willing to put out rather expensive films -- in the chase for prestige and recognition. 

As a newer studio, it makes more sense to avoid this high-risk, end-of-year scramble, and to instead focus on months that seem to be a surer bet. The summer months certainly make sense; people generally have more free time and, perhaps, are looking for an air-conditioned way to spend a few hours. But it also seems that **the springtime** presents an opportunity. There is a slightly higher domestic gross in March, with a similarly higher ROI. This might reflect the fact that spring-breakers have time to spare and are therefore more likely to go to the movies. As a new studio, this could be a good period in which to break into the market.

In `Final.ipynb` we also perform hypothesis testing -- specifically, an ANOVA on the various months of release. The first ANOVA -- regarding gross domestic revenue -- demonstrates that there is, indeed, a statistically significant difference in the gross domestic revenue of movies released in different months; the latter ANOVA -- regarding ROI -- is higher than our chosen $\alpha$, and thus there we cannot reject our null hypothesis. In other words, the second ANOVA shows that there is not a statistically significant difference in average ROI among the different months. Still, we can see there are variations in the means, and can try to draw conclusions accordingly.

### Analysis: 2-D vs. 3-D

We will compare the 3-D movies with 2-D movies based on domestic ROI, domestic gross, and popularity. Looking at ROI and gross will help understand which group may be more profitable, and the popularity metric is also important in order to try to determine which group of movies may help the new studio gain more recognition and media popularity. First, we will create 4 bar charts to compare the means of the 3-D and 2-D movies over these metrics. We include a production budget chart to help explain what we are seeing, as production budget may have an affect domestic gross and popularity.

![ROI 2-D v 3-D](images/roi2d3d.png)

![Gross 2-D v 3-D](images/gross2d3d.png)

![Popularity 2-D v 3-D](images/popularity2d3d.png)

![Production Budget 2-D v 3-D](images/prodbudget2d3d.png)

### Analysis: Experienced vs. Inexperienced Writers & Directors

![Popularity v Director](images/popularitydirector.png)

![Gross v Director](images/GrossDirector.png)

![ROI v Director](images/ROIDirector.png)

![Popularity v Writer](images/PopularityWriter.png)

![ROI v Writer](images/PopularityWriter.png)

### Analysis: Budget

![Budget v Popularity](images/BudgetPop.png)

![Budget v Gross](images/BudgetGross.png)

### Analysis: Runtime

![Runtime v Popularity](images/RuntimePop.png)

![Runtime v Gross](images/RuntimeGross.png)

![Runtime v ROI](images/RuntimeROI.png)

# Conclusions


Our goal has been to provide data-backed recommendations on the best strategy for our client to enter the movie industry. Using three extensive datasets and multiple statistical models, we provide the five recommendations below, each tailored to the resources and interests of a new firm. 


## Summation of Recommendations

**(1.) Time of Release:** 

Spring and summer will be the better times for a newer studio to try to enter the market. Audiences are largest and the most money is available during the summer, but there will be the large summer blockbusters to compete with. Springtime -- and specifically spring break -- presents an opportunity for both high gross revenue and ROI. As a new studio, it probably makes sense to avoid November and December, when big-budget films from major studios are vying for Oscar attention, and would likely crowd out smaller releases. Additionally, later in the year promises much lower ROI than other times -- again, likely because larger studios are willing to swallow losses in the pursuit of prestige.
    
**(2.) 3-D vs. 2-D Movies:** 

We recommend that a new studio avoids 3-D movies. Although we found no significant difference across domestic ROI, domestic gross, and popularity between 3-D movies and 3-D movies, the mean domestic ROI being higher for 2-D movies in our sample may be indicative of higher profitability of 2-D movies when considering the high production budgets of 3-D movies.

**(3.) Experienced Directors and Writers:** 

The experience level of directors and writers does not have a statistically significant effect on domestic ROI. Since experienced directors and writers are more expensive to hire, we recommend that movie studios hire based on salary expectations rather than length of resume. This will keep costs down without sacrificing monetary gain.

**(4.) Budget Recommendation:**

Budget explains about 58% of variance in domestic gross, which means that spending more on a movie is generally a good investment. However, we recognize that our firm may not have as many funds compared to established movie studios. Therefore, we recommend that our firm maximize production value *within* their capabilities.

**(5.) Runtime Recommendation:** 

Runtime has little to no effect on monetary outcomes or movie popularity. When producing a film, our client should focus on remaining within the average/normal length that a viewer expects.


## Potential Next Steps

Going forward, there are a few other ways that we could use this data to provide additional insights for a new studio. We could simply analyze other variables in the data set, such as genre or actor to provide a recommendation about which genre is most profitable to release and which actors or actresses help gain the most media popularity for a new studio. 

There are also ways that we could have manipulated the variables that we analyzed in our project differently. For example, we could have binned the runtimes of our movies in order to approximate the optimal runtime in terms of profitability and popularity of the movie.

Although not in the scope of this project, building a predictive model would also provide more insights about which types of movies will perform best for a new studio.

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
