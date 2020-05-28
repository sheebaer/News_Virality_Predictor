# News_Virality_Predictor
## Data Collection
At present, this predictor crawls a certain news publishing website's pages and gathers all the news articles from there.
The module __BeautifulSoup__ has been used to go through the home page and gather all the links.
These links are then stored in a list and the __newspaper__ module visits these links and gathers details about the article.
All this information is then stored as a JSON file.


## Data Preprocessing
The __Keywords__ present in the article and the __Publishing Date__ of the article have been considered the most important parameters in predicting whether a certain article will go viral or not. The publishing date has been separated into __Publishing Year__, __Publishing Month__, __Publishing Day__ and __Publishing Hour__. To process the data pertaining to keywords, each uniques keyword is assigned a number. The respective keywords are replaced with this number.

Finally, the data is __Normalized__.

## Data Modelling
Since all websites don't publish the number of views on an article, there is not much that can be used to tell if an article has gone viral or not.

So, the approach of __Unsupervised Learning__ has been used. 

The algorithm used here is the __K-Means Clustering Algorithm__.
