# NEWSense - A personalized news article recommendation system

<p align="center">
  <img width="300" height="100" src="https://github.com/akshay-madar/NEWSense-news-recommendation-system-using-twitter/blob/master/NEWSenseLogo.png">
</p>

## Motivation:
Online news reading has exploded as the web provides access to millions of news sources from around the world. The sheer volume of articles can be overwhelming to readers sometimes.
A key challenge for news service websites is to help users to find news articles that are interesting to read. This is advantageous to both users and news service, as it enables the user to rapidly find what he or she needs and the news service to help retain and increase customer base.

## Objective:
To build a hybrid-filtering personalized news articles recommendation product which can suggest articles from popular news service providers based on reading history of twitter users who share similar interests - **Collaborative filtering** and content similarity of the article and user’s tweets - **Content-based filtering**.
This system can be very helpful to Online News Providers to target right news articles to right users.

## But why Twiiter?

<p align="center">
  <img width="400" height="400" src="https://media.giphy.com/media/10zI52A8mrfwNG/giphy.gif">
</p>

### Statistics:
* Twitter has 145 million monetizable daily active users
* 44% of U.S. 18- to 24-year-olds use Twitter
* 71% of Americans on Twitter are using it to read news.

### How Twitter can be used?
Based on user’s tweets we can know user’s interests and can recommend personalized news articles which user would share on Twitter. This can increase news articles and news service’s popularity.

## Fetch twitter data for users
As a first step, the engine identifies readers with similar news interests based on their behavior of retweeting articles posted on Twitter. (Library : Tweepy)

The flow of collecting active users’ data:
  - 1. Fetch users who retweet given News handle's tweets - New York Times, Washington Post and Wall Street Journal. We identify them as  active news readers.
  - 2. Calculate popularity Index = followers count / friends count
  - 3. Filter users based on their twitter activity and popularity (tweets > 10 and popularity > 1)
  - 4. Collect information from Twitter profiles of these filtered active users
