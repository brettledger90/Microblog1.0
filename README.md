# Microblog1.0
------------------------
Part 1
In this project I was able to intsall and do some implementaion with FLASK. I created a virtual environment, and was able to display "Hello World" on the server.

Step one $ brew install pipenv, 
Step two clone the repo and $ cd Microblog1.0
Step three  install python using $ pipenv install --python 3.7
Step four install flask $ pipenv install flask
Step five $ pipenv install flake8


once we have everything installed we are able to see what it actually does, so let's start our venv by first setting it $ export FLASK_APP=microblog.py, once we've set that we can now run a $ flask run , follow the link to the server and get ready for a gasp!
------------------------------------------
Part 2
In part two we will build of part 1 by implamenting some templates, and work with some inherant templates as well.

First I add a base.html, and a index.html
in inserted my code and was able to render a little more with the templates.

To run this, first use $ export FLASK_APP=microblog.py 
then a simple $ flas run should get you off and running.

-------------------------------------------
Part 3 
in part 3 we will start working with web forms.To handle the web forms in this application I'm going to use the Flask-WTF extension, which is a thin wrapper around the WTForms package that nicely integrates it with Flask. This is the first Flask extension that I'm presenting to you, but it is not going to be the last. Extensions are a very important part of the Flask ecosystem, as they provide solutions to problems that Flask is intentionally not opinionated about.

Flask extensions are regular Python packages that are installed with pip. You can go ahead and install Flask-WTF in your virtual environment:

(venv) $ pip install flask-wtf

I then created a login form and rerouted everything.
to run this code simple use $flask run

----------------------------------------------------
Part 4
Databases in Flask
As I'm sure you have heard already, Flask does not support databases natively. This is one of the many areas in which Flask is intentionally not opinionated, which is great, because you have the freedom to choose the database that best fits your application instead of being forced to adapt to one.

There are great choices for databases in Python, many of them with Flask extensions that make a better integration with the application. The databases can be separated into two big groups, those that follow the relational model, and those that do not. The latter group is often called NoSQL, indicating that they do not implement the popular relational query language SQL. While there are great database products in both groups, my opinion is that relational databases are a better match for applications that have structured data such as lists of users, blog posts, etc., while NoSQL databases tend to be better for data that has a less defined structure. This application, like most others, can be implemented using either type of database, but for the reasons stated above, I'm going to go with a relational database.

In Chapter 3 I showed you a first Flask extension. In this chapter I'm going to use two more. The first is Flask-SQLAlchemy, an extension that provides a Flask-friendly wrapper to the popular SQLAlchemy package, which is an Object Relational Mapper or ORM. ORMs allow applications to manage a database using high-level entities such as classes, objects and methods instead of tables and SQL. The job of the ORM is to translate the high-level operations into database commands.

The nice thing about SQLAlchemy is that it is an ORM not for one, but for many relational databases. SQLAlchemy supports a long list of database engines, including the popular MySQL, PostgreSQL and SQLite. This is extremely powerful, because you can do your development using a simple SQLite database that does not require a server, and then when the time comes to deploy the application on a production server you can choose a more robust MySQL or PostgreSQL server, without having to change your application.

To install Flask-SQLAlchemy in your virtual environment, make sure you have activated it first, and then run:

(venv) $ pip install flask-sqlalchemy

Most database tutorials I've seen cover creation and use of a database, but do not adequately address the problem of making updates to an existing database as the application needs change or grow. This is hard because relational databases are centered around structured data, so when the structure changes the data that is already in the database needs to be migrated to the modified structure.

The second extension that I'm going to present in this chapter is Flask-Migrate, which is actually one created by yours truly. This extension is a Flask wrapper for Alembic, a database migration framework for SQLAlchemy. Working with database migrations adds a bit of work to get a database started, but that is a small price to pay for a robust way to make changes to your database in the future.

The installation process for Flask-Migrate is similar to other extensions you have seen:

(venv) $ pip install flask-migrate

then you can run this code by simply using $flask run


