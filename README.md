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
