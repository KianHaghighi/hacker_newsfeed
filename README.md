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

Login/signup route - 
https://dev-cp1a2734d0cenhq1.us.auth0.com/u/login?state=hKFo2SBvTjRUZjFoYkhpSkV1UTVDUkRwRmM3VUpKcW1WWVYya6Fur3VuaXZlcnNhbC1sb2dpbqN0aWTZIEstNWRFWExQYmZLVDBIN2o5bDgtU3NBX0VWWUUwYUw0o2NpZNkgMldvN1d4Z1pqS2tlSXhXZEZ6TVRjSDhGN2lQcUoyaUY

News route(requires user login, will display admin news if admin is logged in, otherwise normal view) - https://www.kianawesomeweb.site/ then login and view the News URL.

News route with JSON objects - https://www.kianawesomeweb.site/newsfeed

Profile page(requires login) - https://www.kianawesomeweb.site/profile 

## Installation

1. Clone the repository:
    ```
    git clone https://gitlab.com/kh21e_fsu/newsfeed.git
    ```
2. Navigate to the project directory:
    ```
    cd news
    ```
3. Install the necessary libraries using the requirements.txt file:
    ```
    pip3 install -r requirements.txt
    pip3 install gunicorn
    sudo apt install nginx
    sudo apt install supervisor 
    ```
4. Start the project
    ```
    sudo supervisorctl restart myproject
    ```

## Configs

This project uses the following configuration files:

- Nginx: Located at '/etc/nginx/sites-enabled/myproject'
- Gunicorn: Located at '/etc/supervisor/conf.d/myproject.conf'

## Testing
To run the web app locally:
    1.navigate to news directory "cd news"
    2.activate the virtual environment "source env/venv/bin/activate"
    3.run the app "python3 app.py"
To run the test cases:
    1.navigate to news directory "cd news"
    2.activate the virtual environment "source env/venv/bin/activate"
    3.run the app "coverage run -m unittest test_app.py"

