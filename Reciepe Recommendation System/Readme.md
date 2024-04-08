## Problem Statement

In this assignment, your objective is to recommend recipes to a user. You have to build a recommender system that will have to generate recommendations for given user_ids.

 

Recommender systems in real life are expected to come up with results instantaneously. Imagine you are surfing YouTube and the recommendations panel to the right of the screen takes 20 minutes to load. That would not be a good experience, and you might decide to use another video streaming service. In the world of recommenders, prediction latency is more important than accuracy. Moreover, the data and features these recommender systems use to make recommendations are very voluminous. The data we used for EDA in the earlier assignment is not on the same scale as the YouTube recommender's data. 

 

How can these recommenders serve recommendations in almost real-time while working on such voluminous data? 
Advanced algorithms. 

The advancements in recommender and deep learning algorithms are responsible for improving prediction latency. 

Use of big data hardware. 

The real-life recommenders use massive hardware clusters to train the algorithms. 


In our case, we will not be able to use deep learning or hardware on the same scale used in the industry. As a result, we will have to sub-sample the data set. 


NOTE: After completing this exercise, you might be tempted to run your machine learning algorithms on the full-scale data you used in the last assignment. We advise against it. You would have to use a large-scale cluster, impacting your AWS credits. 


The data you will work with is given below. 

 

# Downloadable data links 

https://raw-recipes-clean-upgrad.s3.amazonaws.com/raw_ratings_small.csv

https://raw-recipes-clean-upgrad.s3.amazonaws.com/raw_recipies_small.csv

https://raw-recipes-clean-upgrad.s3.amazonaws.com/RAW_recipes_cleaned.csv


# S3 bucket links 

s3a://raw-recipes-clean-upgrad/raw_ratings_small.csv

s3a://raw-recipes-clean-upgrad/raw_recipies_small.csv

s3a://raw-recipes-clean-upgrad/RAW_recipes_cleaned.csv

 

The data file above has the same structure as the data file from the first part of the project. You can refer to the data dictionary from the last project. The data attached here does not have the new features you created earlier, so you must recalculate the features if needed. 


You are expected to use the Spark platform to build your ML model. The algorithms you will use are ALS and K Nearest Neighbors (KNN). 

Note: Using KNN and making a hybrid recommender system will be optional. 

 

You will use the Google Colab environment to solve this assignment. To solve this assignment, you do not need to migrate any data from your AWS account. We have shared the new data files above. You can make a copy of the Google collab template notebooks.
You can download and submit the notebook in .ipynb format. 

If you are new to Google Colab, you can look at this starter notebook; it introduces the Colab environment. It is very similar to your Jupyter notebook. 

 

In the next segment, let's discuss the solution strategy. 

Task List
Task 01: Train Test Split 


As explained earlier, split the interaction data into 80-20 splits based on the review date. For example, if the data has 100 reviews, find a date such that 80 data points are before that date and 20 data points are after. 

 
Task 02: Collaborative Filtering Model

 

1. Build an ALS-based recommender using the native Spark library.  

2. Create 10 recommendations for each user in the test data. 

 
Task 03: KNN models (optional)

    Build a KNN model using the HNSW library 
        Create TFIDF vectors to represent tags of all recipes in the train set. 
        Create user average tag features for the users in the test set.  
    Create 10 recommendations for each user in the test set. 

Task 04: Model Evaluation 

    Evaluate the fit of the ALS model using RMSE. 
    Evaluate the KNN models using (optional)
        Reciprocal rank. 
        nDCG.
        DCG.
         

Task 05: Ensembling Models (optional)

    Scale the numerical outputs of all models to get them into the same scale.
        Think of a strategy to scale the output such that the variation of values is not lost. 
    Combine the recommendations of all KNN models. 
    Combine the recommendation of all KNN and ALS models. 