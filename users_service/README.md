This project contains Rest microservice written in Flask for managing users.

## Instalation
Go to project directory and then:
`pip install -r requirements.txt`

## Configuration and Launching
Set enviroment variable USERS_CONFIG with one of values:
 * development - for developing,
 * testing - for run tests,
 * production - on the production server

Then `python manage.py migrate` for run application
or `python manage.py test` run tests.

## Endpoints:
* GET /users - gets list of all users
* POST /users - add new user in format `{"name": "John Smith"}`
* GET /users/<user_id>  - remove user by his id
