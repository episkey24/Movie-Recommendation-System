## Movie Recommendation System
UCS757 - Building Innovative Systems. <br />
Project - 1 <br />
[Live Link](https://ucs757-p1-mrs-101803201.herokuapp.com/) 
### Overview
This Movie Recommendation System uses Content-Based filtering approach to determine movie recommendations and movie details are also displayed based on user search. <br />
Web scraping is used to get user reviews which are then classified using multinomial Naive Bayes classifier.  <br />
It is created using Flask web framework and is deployed on Heroku. <br />
(Preprocessed data enclosed in this github-repo as main_data.csv)
### Methodology
![Flowchart](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(79).png)
### Screenshots
![Home Page](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(73).png) <br />
![Details](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(74).png) <br />
![Reviews](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(76).png) <br />
![Recommendations](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(77).png)
### Tech Stack
- [React.js](https://github.com/facebook/react) is used for Frontend.
- [Flask](https://github.com/pallets/flask) is used in the backend. The API endpoint for getting the recommmendations is setup with cross-site-origin access.
- [Scikit Learn Count-Vectorizer](https://github.com/scikit-learn/scikit-learn) Scikit-Learn's CountVectorizer is used for preperation of the Recomendeer system. The Cosine similarity parameter is used for finding the closest neigbhours. The top 10 movies with closest similarity score are selected.
- [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) python package is used for web scraping the movie reviews from IMBD and to classify them, sentiment analysis is performed for which [multinomial Naive Bayes classifier](https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html) provides an accuracy of about 97.47%.
- [Tmdb](https://github.com/gajus/tmdb) is used to fetch the attribute information and image data of movies and recommendations accoriding to official IMDB's records.
- [Heroku](https://github.com/heroku/heroku-buildpack-python) The application is deployed live on Heroku, using gunicorn static-file web server.
### Install and Run on your Machine:
- Clone this repository or download the zip file.
- Install the requirements using: ``` pip install -r requirements.txt ```
- To start the app on the localhost move to the respective directory, run the command: ``` python main.py ```

If you want to remake the ML model, you can use the already preprocessed data enclosed in this github-repo as main_data.csv .
