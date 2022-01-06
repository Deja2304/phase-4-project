# Movie Recommendations

**Authors**: Deja Prade, Emiko Naomasa

## Overview

In this project, we build a movie recommendation system using the MovieLens ratings data set. We develop a content-based recommendation model for recommendations to new customers and a collaborative filtering model for recommendations to existing customers. Using our model, we provide the top five movie recommendations for new and existing customers. 


## Business Understanding 
Popcorn (our stakeholder) is a startup company that recently entered the movie streaming business. The video streaming market is rapidly growing worldwide. To compete with the market giants, such as Netflix, Hulu, or Amazon Prime, Popcorn tasked us to build for their platform a movie recommendation system. This recommendation engine is a powerful tool, especially for the video streaming business.  For example, more than 80 percent of shows watched on Netflix came from Netflix recommendations. In this context, our project aims to develop a movie recommendation system for Popcorn that can effectively recommend movies and maximize customer satisfaction with Popcorn’s streaming service. 


## Data
We use the [MovieLens data set](https://grouplens.org/datasets/movielens/). This data set (ml-latest-small) contains 102,377 ratings (5-star rating) and 3,476 tag applications created between March 29, 1996, and September 24, 2018. A total of 610 users and 9,742 movies are included. 

The data set also includes movie genres (Action, Adventure, Animation, Children’s, Comedy, Crime, Documentary, Drama, Fantasy, Film-Noir, Horror, Musical, Mystery, Romance, Sci-Fi, Thriller, War, Western, and (no genres listed)). 

All users had rated at least 20 movies. No demographic information is provided.


## Model
We develop **a content-based recommendation model** based on movie genres and **a collaborative filtering model** based on user ratings. Content-based and collaborative filtering are two of the most common types of recommendation systems. Content-based recommendation systems focus on the items’ attributes, such as genres, and provide recommendations based on the similarity between them. In contrast, the collaborative filtering recommender is entirely based on a viewer’s history and not the context. It analyses how similar the taste of one user is to another and makes recommendations on that basis. 
Because collaborative filtering has a cold start problem, for the case of new users or new items, we build a content-based recommender. For the existing users, we build a collaborative filtering model. 

![image](https://user-images.githubusercontent.com/38669459/148383995-1d35687f-f2b1-49e1-abb9-7a113d2e534a.png)



For model creation and evaluation, please read our jupyter notebook. (For [content-based recommendation model] and for [collaborative filterling model](https://github.com/Deja2304/phase-4-project/blob/main/2_Collaborative_Filtering_Recommendation.ipynb).)


## Model Evaluation
We assessed our movie recommendation system by examining the derived top 5 movie recommendations for real users in our samples and a new user (an author). In general, our recommendations for existing customers seemed not far from their preferences. For content based filtering our recommendations were aligned as well, some happened to be movies Deja had already seen.


### Recommendations for Existing Customer

### Recommendations for New Customer
Based of ratings given for The Omen, Higher Learning, Waiting To Exhale, Exorcist, Mission Impossible, Final Destination, and Predator these were the recommendation given. 

<img width="756" alt="Screen Shot 2022-01-05 at 2 04 08 PM" src="https://user-images.githubusercontent.com/92389914/148460693-f4c386d4-0fdb-44ad-8cbc-d163b6a5b5ff.png">



## Conclusion
A limitation in our recommendation system is that if a person had a unique taste, the collaborative filtering might not provide a good recommendation. Because this model is based on the similarity with other users, a person who had very different preference from others may not receive any reasonable recommendations. 
Additionally, in our dataset, over 75% of movies received fewer than 10 reviews. Our model put less weight on these less-rated movies. As a consequence, a small portion of popular movies are often recommended, and an unpopular movie would remain invisible for a long time. 


Next Step 
- Develop a hybrid model, combining content-based and collaborative filtering models. 
- For the content-based model, explore other movie features, such as tags, directors. 
- For the collaborative filtering model, use timestamp data to weigh recent ratings, thereby reflecting the recent user’s trends.  
- Used a larger dataset from the movie lens and checked scalability. 
- Conduct A/B testing to assess whether a person really watches a recommended movie. 
- Filter for movies with same title


## For More Information 
Please review our full analysis in our Jupyter Notebook or our presentation.
For any additional questions, please contact: [Deja Prade](https://www.linkedin.com/in/deja-prade/), [Emiko Naomasa](https://www.linkedin.com/in/emiko-n-58782158/) 



## Repository Structure

```
├── README.md                           <- The top-level README for reviewers of this project
├── Notebook.ipynb                         <- Concise summary of the project with all data science steps
├── Project 4.pdf                       <- PDF version of project presentation
├── Data                                <- Both sourced externally and generated from code, includes exploratory notebooks
└── Images                              <- Both sourced externally and generated from code
```  
Note: Large or sensitive files are listed in .gitignore and not pushed to GitHub.
