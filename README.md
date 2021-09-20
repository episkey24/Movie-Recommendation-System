## Movie-Recommendation-System
UCS757 - Building Innovative Systems. <br />
Project - 1 <br />
[Live Link](https://ucs757-p1-mrs-101803201.herokuapp.com/)
### Overview
This Movie Recommendation System is created using Flask web framework and deployed on Heroku. 
It uses Content-Based filtering approach to determine movie recommendations based on user search.
### Characteristic Functionalities
-
-
-
### Tech Stack
- [React.js](https://github.com/facebook/react) is used for Frontend.
- [Flask](https://github.com/pallets/flask) is used in the backend. The API endpoint for getting the recommmendations is setup with cross-site-origin access.
- [Scikit Learn Count-Vectorizer](https://github.com/scikit-learn/scikit-learn) Scikit-Learn's CountVectorizer is used for preperation of the Recomendeer system. The Cosine similarity parameter is used for finding the closest neigbhours. The top 10 movies with closest similarity score are selected.
- [Tmdb](https://github.com/gajus/tmdb) is used to fetch the attribute information and image data of movies and recommendations according to official IMDB's records.
- [Heroku](https://github.com/heroku/heroku-buildpack-python) The application is deployed live on Heroku, using gunicorn static-file web server.
