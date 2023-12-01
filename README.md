In order to run the flask app:
    1.navigate to news directory "cd news"
    2.activate the virtual environment "source env/venv/bin/activate"
    3.run the app "python3 app.py"

# Project Name - Newsfeed

## Description
The project is a Python web application that displays news from the Hacker News portal. It includes pages for Sign Up/Login, News Feed, Profile, and Admin functionalities. Users can like or dislike news items, and the application sorts news by time and popularity. Admin can delete news and the related likes and dislikes from the database.

Video Demonstration URL: https://www.youtube.com/watch?v=lCFgIwiJMLE

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Configs](#configs)
- [Testing](#testing)

## Features

- List key features of your web application with URLS.

Login route - https://dev-cp1a2734d0cenhq1.us.auth0.com/u/login?state=hKFo2SBvTjRUZjFoYkhpSkV1UTVDUkRwRmM3VUpKcW1WWVYya6Fur3VuaXZlcnNhbC1sb2dpbqN0aWTZIEstNWRFWExQYmZLVDBIN2o5bDgtU3NBX0VWWUUwYUw0o2NpZNkgMldvN1d4Z1pqS2tlSXhXZEZ6TVRjSDhGN2lQcUoyaUY

News route(requires user login, will display admin news if admin is logged in, otherwise normal view) - https://www.kianawesomeweb.site/news

News route with JSON objects - https://www.kianawesomeweb.site/newsfeed

Profile page(requires login) - https://www.kianawesomeweb.site/profile 
## Installation

List down all the steps from setting up a server to hosting your application with Nginx and Gunicorn with all necessary libraries. Include a requirements.txt for setting up the environment easily.


## Configs
All the necessary configuration files (Nginx, supervisor, Gunicorn, Cron etc) you need to setup your server and web application. Please exclude any kind of personal information. 


## Testing
All the necessary steps to run testcodes in your repository.
    1.navigate to news directory "cd news"
    2.activate the virtual environment "source env/venv/bin/activate"
    3.run the app "coverage run -m unittest test_app.py"

