# Flaskr Blog 
Flaskr is a basic blog app developed with Flask micro framework, as a part of [this Flask tutorial](https://flask.palletsprojects.com/en/1.1.x/tutorial/).

It has the basic CRUD functionality and it uses SQLite database to store users and posts.
## Install

Clone this repository and cd to the project folder.


Create a virtualenv and activate it:

    $ python3 -m venv venv
    $ . venv/bin/activate

Or on Windows cmd:

    $ py -3 -m venv venv
    $ venv\Scripts\activate.bat

Install Flaskr:

    $ pip install -e .


## Run

    $ export FLASK_APP=flaskr
    $ export FLASK_ENV=development
    $ flask init-db
    $ flask run

Or on Windows cmd:

    > set FLASK_APP=flaskr
    > set FLASK_ENV=development
    > flask init-db
    > flask run

Open http://127.0.0.1:5000 in a browser.

## Test
    $ pip install '.[test]'
    $ pytest

Run with coverage report:

    $ coverage run -m pytest
    $ coverage report
    $ coverage html  # open htmlcov/index.html in a browser
