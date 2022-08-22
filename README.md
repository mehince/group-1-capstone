# How to Navigate this Repository

Our final notebook can be found in the file __Finalized Notebook.ipynb__ and contains 
the data exploration, cleaning and analysis that supported our final recommendations for Computer Vision. 

The data we used to complete our analysis is located in the __zippedData__ folder. 

Regaring the IMDB dataset, there is an entity-relationship diagram that outlines how data is organized in the __im.db.zip__ file. We primarily used the __movie_basics__ and __movie_ratings__ tables to conduct our analysis.  

# Relevant Links
* [Presentation]()
* [Box Office Mojo](https://www.boxofficemojo.com/)
* [The Numbers](https://www.the-numbers.com/)
* [IMDB](https://www.imdb.com/)

# Overview 

Computer Vision wants to break into the movie production industry, but needs insight regarding what types of movies to make. 

We have recommended three courses of action for Computer Vision to follow that will allow their films to be successful at the box office:
* Produce a movie in the animation genre (with the possibility of a comedy sub-genre).
* Allocate $80 million towards movie production. 
* Allocate more marketing effort towards international audiences (rather than domestic audiences). 

We based these recommendations off three high-priority metrics:
* Highest-rated movie genres
* Budget-to-box office ratio
* Which production studios gross the highest
  ** Which genres of movies these production studios produce

# Business Understanding 

* Computer Vision wants to establish a movie studio to create video and movie content. 
* Computer Vision is new to the movie / video market, and needs guidance regarding what types of movies to create. 
* Providing insights into what types of movies are doing best at the box office will allow Computer Vision to allocate their budget towards creating a successful film. 

# Data Understanding 

We used data from three main sources to make recommendations for Computer Vision:
* Box Office Mojo
* The Numbers
* IMDB (Internet Movie Database)

The data from Box Office Mojo included movie domestic and foreign gross, and movie production studio.
* Dataset contained in a .csv file
* Approximately 39% missing data in foreign gross column

Data from The Numbers included production budget and worldwide gross information.
* Dataset contained in a .csv file
* Approximately 6% missing data in worldwide gross

Data from IMDB included general movie information such as title, average ratings, and genres.
* Data represented as a relational SQL database
* Most analysis done using **movie_basics** and **movie_ratings** tables

We only considered movies in each dataset that had been released in 2010 or later.

# Data Analysis

We used three high-priority metrics to focus our analysis. These metrics were:
* Highest-rated movie genres
* Budget-to-box office ratio
* Which production studios gross the highest
  * Which genres of movies these production studios produce
 
We cleaned, aggregated, and normalized data from Box Office Mojo, The Numbers, and the Internet Movie Database (IMDB) to calculate these metrics and create recommendations for Computer Vision. We also used hypothesis testing to determine whether Computer Vision should market their movies in the international or domestic spaces. 

# Statistical Communication

After identifying **animation** as the genre Computer Vision should pursue, we wanted to explore the difference between the genre's foreign and domestic gross. Specifically, we hypothesize that the animation genre will gross higher internationally than domestically. Based on the results of the test we can determine where to best spend marketing efforts to maximize profitability.

The results of our statistical test show that with 95% confidence foreign gross is significantly greater than domestic gross in the Animation genre. This indicates that more money should be spent marketing to foreign markets as opposed to domestic.  

# Conclusion
### Summary of Recommendations

* Computer Vision should produce a movie in the animation genre.
* Computer Vision should spend approximately $80 million on the production of their first movie. 
* Computer Vision should allocate more marketing effort and funds towards the international market versus the domestic market. 

### Next Steps

* We would like to continue to test our hypothesis and compare our recommendations to those that would be produced from the datasets we did not use. 
* We would like to collect more revent movie rating and box office data for more rigorous analysis. 
* We would like to conduct further analysis regarding how much money should be allocated towards international versus domestic marketing efforts.
