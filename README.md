# Djangular_UserAuth
Basic registration, login and logout application using Django, REST and AngularJS


## Installation

*NOTE: Requires [virtualenv](http://virtualenv.readthedocs.org/en/latest/),
[virtualenvwrapper](http://virtualenvwrapper.readthedocs.org/en/latest/), [postgress](http://www.postgresql.org/download/macosx/) and
[Node.js](http://nodejs.org/).*

* Fork this repository.
* `$ git clone git@github.com:<your username>/Djangular_UserAuth.git`
* `$ mkvirtualenv APP_NAME`
* `$ cd Djangular_UserAuth/`
* `$ pip install -r requirements.txt`
* `$ npm install -g bower`
* `$ npm install`
* `$ bower install`
* If the DB isn't running, in the virtualenv, run <code>postgres -D /usr/local/var/postgres</code>
* In the virtualenv,  <code>psql postgres</code>
* In postgres, open <code>create database PROJECT_NAME;</code>
* In <code>local_settings.py</code> edit <code>PROJECT_NAME</code> to match your database name
````Python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'PROJECT_NAME',
    }
}
````

* `$ python manage.py migrate`
* `$ python manage.py runserver`
