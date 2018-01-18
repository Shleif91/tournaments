HABB tournaments project 
========================

Create docker container:
------------------------
1. `docker-compose build`
2. `docker-compose up`

Create database
------------
1. `docker-compose exec web bash`
2. `python manage.py migrate`

Create admin
------------
1. `docker-compose exec web bash`
2. `python manage.py createsuperuser`

Get tables from database
------------------------
1. `docker-compose exec db bash`
2. `psql -U postgres -d postgres`
3. `\dt`