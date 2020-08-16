Fyyur
Introduction
Fyyur is a musical venue and artist booking site that facilitates the discovery and bookings of shows between local performing artists and venues. This site lets you list new artists and venues, discover them, and list shows with artists as a venue owner.

Tech Stack
SQLAlchemy ORM to be our ORM library of choice
PostgreSQL as our database of choice
Python3 and Flask as our server language and server framework
Flask-Migrate for creating and running schema migrations
HTML, CSS, and Javascript with Bootstrap 3 for our website's frontend
Main Files: Project Structure
├── README.md
├── app.py *** the main driver of the app. 
                  "python app.py" to run after installing dependences
├── config.py *** Database URLs, CSRF generation, etc
├── error.log
├── forms.py ***  Forms
├── models.py  *** SQL Alchemy models
├── requirements.txt 
├── static
│   ├── css 
│   ├── font
│   ├── ico
│   ├── img
│   └── js
└── templates
    ├── errors
    ├── forms
    ├── layouts
    └── pages
Development Setup
First, install Flask if you haven't already.

$ cd ~
$ sudo pip3 install Flask
To start and run the local development server,

Initialize and activate a virtualenv:
$ cd YOUR_PROJECT_DIRECTORY_PATH/
$ virtualenv --no-site-packages env
$ source env/bin/activate
Install the dependencies:
$ pip install -r requirements.txt
Run the development server:
$ export FLASK_APP=myapp
$ export FLASK_ENV=development # enables debug mode
$ python3 app.py
Navigate to Home page http://localhost:5000
