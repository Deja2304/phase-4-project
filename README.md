# Movie Recommendations


**Authors**: Deja Prade, Emiko Naomasa

## Overview
In this project, we build a movie recommendation system using the MovieLens ratings data set. We develop a content-based recommendation model for recommendations to new customers and a collaborative filtering model for recommendations to existing customers. Using our model, we provide the top five movie recommendations for new and existing customers. 


## Business Understanding 
Popcorn (our stakeholder) is a startup company that recently entered the movie streaming business. The video streaming market is rapidly growing worldwide. To compete with the market giants, such as Netflix, Hulu, or Amazon Prime, Popcorn tasked us to build for their platform a movie recommendation system. This recommendation engine is a powerful tool, especially for the video streaming business.  For example, more than 80 percent of shows watched on Netflix came from Netflix recommendations. In this context, our project aims to develop a movie recommendation system for Popcorn that can effectively recommend movies and maximize customer satisfaction with Popcorn’s streaming service. 


## Data
We use the [MovieLens data set](https://grouplens.org/datasets/movielens/). This data set (ml-latest-small) includes 5-star rating and free-text tagging activity. It contains 102,377ratings and 3,476 tag applications across 9,742 movies. A total of 610 users created these ratings between March 29, 1996, and September 24, 2018. 
All users had rated at least 20 movies. No demographic information is provided.


## Model
We develop **a content-based recommendation model** based on movie genres and **a collaborative filtering model** based on user ratings. Content-based and collaborative filtering are two of the most common types of recommendation systems. Content-based recommendation systems focus on the items’ attributes, such as genres, and provide recommendations based on the similarity between them. In contrast, the collaborative filtering recommender is entirely based on a viewer’s history and not the context. It analyses how similar the taste of one user is to another and makes recommendations on that basis. 

Because it relies on a person’s rating/viewing history, collaborative filtering has a cold start problem. When a new user joins a streaming platform, the model cannot make any personal recommendations. When a new movie arrives, until a substantial number of users rate it, the model cannot make a recommendation. Thus, for the case of new users or new items, we build a content-based recommender. It relies on features, not on a person’s viewing history.

For model creation and evaluation, please read our jupyter notebook. (For [content-based recommendation model] and for [collaborative filterling model] <-add link)


## Recommendations for Existing Customer

## Recommendations for New Customer


## Conclusion


## For More Information 
Please review our full analysis in our Jupyter Notebook or our presentation.
For any additional questions, please contact: [Deja Prade](-add linkedin), [Emiko Naomasa](https://www.linkedin.com/in/emiko-n-58782158/) 



## Repository Structure

```
├── README.md                           <- The top-level README for reviewers of this project
├── Notebook.ipynb                         <- Concise summary of the project with all data science steps
├── Project 4.pdf                       <- PDF version of project presentation
├── Data                                <- Both sourced externally and generated from code, includes exploratory notebooks
└── Images                              <- Both sourced externally and generated from code
```  
Note: Large or sensitive files are listed in .gitignore and not pushed to GitHub.
