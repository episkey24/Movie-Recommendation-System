## Movie Recommendation System
UCS757 - Building Innovative Systems. <br />
Project - 1 <br />
[Live Link](https://ucs757-p1-mrs-101803201.herokuapp.com/) 
### Overview
This Movie Recommendation System is created using Flask web framework and deployed on Heroku. <br />
It uses Content-Based filtering approach to determine movie recommendations based on user search. <br />
(Sample Data already enclosed in this github-repo)
### Screenshots
![Home Page](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(73).png) <br />
![Details](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(74).png) <br />
![Recommendations](https://github.com/episkey24/Movie-Recommendation-System/blob/main/Screenshots/Screenshot%20(77).png)
### Tech Stack
- [React.js](https://github.com/facebook/react) is used for Frontend.
- [Flask](https://github.com/pallets/flask) is used in the backend. The API endpoint for getting the recommmendations is setup with cross-site-origin access.
- [Scikit Learn Count-Vectorizer](https://github.com/scikit-learn/scikit-learn) Scikit-Learn's CountVectorizer is used for preperation of the Recomendeer system. The Cosine similarity parameter is used for finding the closest neigbhours. The top 10 movies with closest similarity score are selected.
- [Tmdb](https://github.com/gajus/tmdb) is used to fetch the attribute information and image data of movies and recommendations accoriding to official IMDB's records.
- [Heroku](https://github.com/heroku/heroku-buildpack-python) The application is deployed live on Heroku, using gunicorn static-file web server.
### Install and Run on your Machine:
- Clone this repository or download the zip file.
- Install the requirements using: pip install -r requirements.txt
- To start the app on the developement server move to the respective directory, run the command: python main.py

If you want to remake the ML model, you can use the already preprocessed data enclosed in this github-repo as main_data.csv .
