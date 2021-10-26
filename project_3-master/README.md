# Project 3: Sucessful SEO 
---

### Contents:

- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Data Sources](#Data-Sources)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

---

### Problem Statement:

Search Engine Optimization, abbreviated as SEO is the process of improving a website to increase visibility for relevant searches. Google is the most popular search engine in the world and digital marketing is one of our most important marketing channels at House Depot. Currently, we are ranked at number 5 on google when you search our name and also our top products. SEO, is using strategies to improve visbility and targets organic and unpaid traffic. This is important, since we can optimize our position on google for free and increase brand awareness and customer acquistion. But where do we start on improving our SEO? This is where Data Science can help. I will examine what keywords we can use to optimize our webpage. 



### Executive Summary

For this analysis, I collaborated with the sales team to determine our top selling products. These products include HousePlants and Interior Design elements. The next step, was to find a data source. In digital marketing, you want to go where the customers are. Reddit, the social news platform where users can discuss topics and vote was chosen as the source of our data. This data is readily available for free through the push shift API. We have chosen the House Plants subreddit and the Interior Design subreddit, and collected around 10,000 posts. For our analysis, we only focused on the titles due to titles and google search words are highly correlated. We discovered the top 20 most frequently used words in a combination of posts from both subreddits. Then we created a classification model using machine learning, to ensure we are choosing the right words. This was done after dropping all missing values, using a Count Vectorizer to transform the text into numerical data to give to the machine to predict a class, House Plants or Interior Design. Our best performing model included using this process and the algorithm Multi Nomial Naive Bayes Classifier. 



### Data Sources
* [`combined.csv`](./data/combined.csv): Combined Interior Design and House Plants Subreddits, including 'title column, selftext and title word count



### Conclusions and Recommendations
In conclusion, we will focus on four GO words, (Google Optimization). These words are apart of the top 20 most frequently mentioned words. Our GO words include help, plant, design and new home. Our classification model has a 94% accuracy score on unseen (testing) data. We will implement the use of these GO words in all of our marketing campaigns. The next step in our strategy is to update our website and clean up HTML/CSS codes and add in GO words to improve our position on google. 