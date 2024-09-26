# movie_recommendation_system
This project is a Movie Recommendation System built in Python that recommends movies based on the content features of other movies. It uses the content-based filtering approach, where the recommendation is made by analyzing movie features such as genres, keywords, cast, director, and overview.

## Libraries
Pandas: For loading and preprocessing the dataset.

Scikit-learn: For transforming text features into numerical vectors and calculating similarity.

Difflib: For finding the closest match for the input movie title.

TfidfVectorizer: From Scikit-learn to convert text data into feature vectors based on Term Frequency-Inverse Document Frequency.

Cosine Similarity: A metric used to determine the similarity between movies.

## Steps
1. Loading Data: The project begins by loading the movies.csv dataset containing movie metadata.
Preprocessing: Null values in the relevant features (genres, keywords, tagline, cast, director, and overview) are filled with empty strings to avoid errors during processing.

2. Combining Features: The selected features are combined into a single string for each movie, allowing the algorithm to process all relevant information at once.

3. Vectorizing Text: The combined text is converted into feature vectors using TF-IDF (Term Frequency-Inverse Document Frequency) to numerically represent the movie features.

4. Calculating Similarity: Cosine similarity is calculated between the vectors of all movies to determine how similar each movie is to the others.

5. Recommending Movies: When a user inputs a movie title, the system finds the closest match in the dataset and retrieves a list of similar movies based on the cosine similarity scores.

### Link to dataset
https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view
