# Recommender-System-using-Community-Detection-and-Probabilistic-Matrix-Factorization
The Community-Based Probabilistic Matrix Factorization (CBPMF) model consists of two main components: community detection and probabilistic matrix factorization. 
In the community detection phase, a community-detection algorithm is used to identify overlapping communities within a social network based on common interests. This algorithm analyzes user interactions and identifies groups of users who share similar preferences or behaviors. 
The probabilistic matrix factorization (PMF) component is trained using the stochastic gradient descent algorithm. It predicts ratings for items based on the user-item interactions. 
The model is applied to generate recommendations by predicting ratings for items that have not been rated yet. 
The proposed CBPMF model incorporates community information to enhance the prediction of ratings for unrated items. 
The model calculates cosine similarity scores between pairs of users and constructs a similarity matrix, which acts as a weight matrix for detecting overlapping communities. 
The overlapping communities are then used to recommend items to users using the PMF model. 
For each user, the model determines the number of communities the user belongs to. It creates a user-item rating matrix for each community, which is then factorized using PMF to estimate the unobserved ratings for each item within that community. 
The highest predicted rating value is selected and updated in the item list for that user. 
Finally, the top-N items with the highest predicted ratings are recommended to the user. The recommendation algorithm leverages the idea that users within the same community tend to have similar preferences or behaviors. 
By considering community preferences, personalized recommendations are provided to each user. Overall, the CBPMF model combines community detection and probabilistic matrix factorization to generate accurate and personalized recommendations based on user-community preferences
