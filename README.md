# Python: api-sisben

![](https://scontent.fbaq1-1.fna.fbcdn.net/v/t1.0-9/149050605_1007355226458515_1684189489609037716_n.jpg?_nc_cat=101&ccb=3&_nc_sid=730e14&_nc_eui2=AeGxx263aNaqLUwaua17K_8I1EsLvf8wotTUSwu9_zCi1FgPV4273dBCqQ9wAimpNM6pX1i5b4wasexfQsjQOLh_&_nc_ohc=5twQ0uGsN2oAX9bwbnM&_nc_ht=scontent.fbaq1-1.fna&oh=1d3cd6e09d2a1820f1e879c62a1ed1f3&oe=604973EF)

A barebones Django app, which can easily be deployed to Heroku.

This application supports the [Getting Started with Python on Heroku](https://devcenter.heroku.com/articles/getting-started-with-python) article - check it out.

## Running Locally

Make sure you have Python 3.9 [installed locally](http://install.python-guide.org). To push to Heroku, you'll need to install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli), as well as [Postgres](https://devcenter.heroku.com/articles/heroku-postgresql#local-setup).

```sh
$ git clone https://github.com/Esteban1891/api-sisben
$ cd backend

$ python3 -m venv venv
$ pip install -r requirements.txt

$ createdb backend

$ python manage.py migrate
$ python manage.py collectstatic

$  heroku local -p 7001  
```

Your app should now be running on [localhost:7001](http://localhost:7001/).

## Deploying to Heroku

```sh
$ heroku create
$ git push heroku master

$ heroku run python manage.py migrate
$ heroku open
```
or

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Documentation

For more information about using Python on Heroku, see these Dev Center articles:

- [Python on Heroku](https://devcenter.heroku.com/categories/python)
# deploy
