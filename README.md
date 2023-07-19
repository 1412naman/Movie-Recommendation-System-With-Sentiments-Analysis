# Movie-Recommendation-System-With-Sentiments-Analysis

Discover personalized movie suggestions using sentiment analysis! Our user-friendly system recommends films aligned with your emotions and preferences. 🎬🍿
The details of the movies(title, genre, runtime, rating, poster, etc) are fetched using an API by TMDB, https://www.themoviedb.org/documentation/api, and using the IMDB id of the movie in the API, I did web scraping to get the reviews given by the user in the IMDB site using beautifulsoup4 and performed sentiment analysis on those reviews.
Check out the live demo:
Link to youtube demo:
# FlixiFy
Welcome to Flixify, your ultimate movie companion! Flixify is an intelligent movie recommendation system that utilizes sentiment analysis and TMDB ratings to offer personalized film suggestions tailored to your preferences. Whether you're seeking heartwarming romances, adrenaline-pumping adventures, or gripping thrillers, Flixify has you covered.
![Uploading Screenshot 2023-07-19 at 9.42.24 PM.png…]()



# How to get the API key?
Create an account at https://www.themoviedb.org/, click on the API link from the left-hand sidebar in your account settings and fill in all the details to apply for the API key. If you are asked for the website URL, give "NA" if you don't have one. Once your request is approved, you will see the API key in your API sidebar.
# How to run the project?
1. Clone or download this repository to your local machine.
2. Install all the libraries mentioned in the requirements.txt file with the command `pip3 install -r requirements.txt`
3. Get your API key from https://www.themoviedb.org/. (Refer to the above section on how to get the API key)
4. Replace YOUR_API_KEY in both places (lines no. 15 and 29) of the `static/recommend.js` file and hit save.
5. Open your terminal/command prompt from your project directory and run the file main.py by executing the command `python3 main.py`.
6. Go to your browser and type `http://127.0.0.1:5000/` in the address bar.
7. Hurray! That's it.
!!Always go with the latest versions of requirements.

# Similarity Score :
How does it decide which item is most similar to the item user likes? Here come the similarity scores.

It is a numerical value that ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained by measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.

# How does Cosine Similarity work?
Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, the higher the cosine similarity.

![image](https://github.com/1412naman/Movie-Recommendation-System-With-Sentiments-Analysis/assets/114249251/be24e112-0a43-446e-ac45-575175c1accd)

# Sources of the datasets
1. https://www.kaggle.com/datasets/carolzhangdc/imdb-5000-movie-dataset
2. https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset
3. https://en.wikipedia.org/wiki/List_of_American_films_of_2018
4. https://en.wikipedia.org/wiki/List_of_American_films_of_2019
5. https://en.wikipedia.org/wiki/List_of_American_films_of_2020
6. https://en.wikipedia.org/wiki/List_of_American_films_of_2021
7. https://en.wikipedia.org/wiki/List_of_American_films_of_2022
8. https://en.wikipedia.org/wiki/List_of_American_films_of_2023
