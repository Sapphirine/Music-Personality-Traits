# Music-Personality-Traits
This project aims at deriving personality traits from music related data and uses the performance of the recommender system to evaluate the potential influence of music preferences of users. 

# Workflow of the code
1. Start the project by running the file UserProfile.ipython. It contains the whole personality derivation pipeline. It takes csv or similar files as input and outputs a dictionary containing selected users with corresponding dominant music preferences in the form of a pickle file. 
2. Then run the file RecEvaluation.ipython to read the main dataset and the resulting pickle file from the previous step. It evaluates the performance of the recommender system using Spark MLlib packages and uses NDCG as its evaluation metrics among different groups of users categorized by their dominant music preferences. 

# Accessibility
Even though the files in the repository take csv or similar files as inputs, it is easy to transform your own datasets to use the pipeline and the evaluation step. 

# Dataset
The original dataset used in this project is gained from the website: http://ocelma.net/MusicRecommendationDataset/lastfm-360K.html
It is gained from Last.fm API and collected by Oscar Celma. 
