Install dependencies:

Install  Django 3.1 and pip first

(while in the activated virtual environment)

pip install -r requirements.txt


Migrate, create a superuser, and run the server:

python manage.py makemigrations

python manage.py migrate

python manage.py createsuperuser

python manage.py runserver

PostgreSQL Setup : 

    Download postgresql setup form https://www.postgresql.org/download/
    Download pgadmin setup from https://www.pgadmin.org/download/
    Start pgadmin and make a new database.

Security settings for Postgresql : 

Open the DjangoProject/settings.py file and change USER and PASSWORD here:

DATABASES = {

    'default': {

        'ENGINE': 'django.db.backends.postgresql',

        'NAME': 'carzone_db',
        'USER': 'postgres',
        'PASSWORD' : 'desktop',
        'HOST': 'localhost',
    }
}
