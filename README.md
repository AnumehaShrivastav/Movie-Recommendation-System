# Movie-Recommendation-System
A recommender system is a type of information filtering system. By drawing from huge data sets, the system’s algorithm can pinpoint accurate user preferences. As part of this project, We are building A content based movie recommender system using cosine similarity.

## Types of recommender system:
1. Content-based recommendation
2. Collaborative Filtering
3. Hybrid recommender system

## Approach Used :
Content-based Filtering- This approch uses attributes such as title, overview, genre, director, actors for movies, to make suggestions for the users. The intuition behind this sort of recommendation system is that if a user liked a particular movie, User might like a movie or a show similar to it.

## Project Flow:
Data Collection >> Preprocessing >> Model building >> Website >> Deployment

### Data Set
The data set used for this notebook is taken from below two sources:
1. Collected data by Scraping bunch of Wikipedia pages (Latest movies)
2. TMDB-5000 movie dataset

The dataset can be found here : [disney_movie_dataset_final.csv](https://github.com/AnumehaShrivastav/Movie-Recommendation-System/files/8596779/disney_movie_dataset_final.csv) , 
[Uploading tmdb_5000_movies.csv…]()

## Data Preprocessing
1. Mearged both the dataframes
1. Feature selection
2. Handling NAN values
3. Used an API to add some additonal info to the dataset
4. Concadinated all the coulumn to create the Tags

## Model building
We need to calculate the similarity score belween tags
1. Text Vectorization Techniques- Bags of words, tfidf, word2vec. We are using CountVectorizer
2. Select hyperparameters- max_features, Stop_words etc..
3. Apply Stemming process to get root of words in order to avoid duplicate features
4. Calculate cosine similarity between vectors
5. Define a function which returns 5 similar movies for a given movie based on similarity matrix

## Website
1. Use Pycharm IDE and create new project (Create venv)
2. Use Flask/Streamlit library
3. Create app.py file
4. run the app by streamlit run app.py
5. Deploy the model on Heroku server (Platform as services)

## Required Tools
1. SKlearn
2. Numpy
3. Pandas
4. Scipy
5. python
6. BeautifulSoup
7. Requests
8. NLTK
