# django-polls-tutorial

This is the solution code to the [Django official tutorial](https://docs.djangoproject.com/en/4.0/intro/tutorial01/), using:

    $ python3 -V && echo -n 'Django ' && python3 -m django --version
    Python 3.9.9
    Django 4.0.2

# First time

    mkdir ~/.virtualenv-3.9.9
    virtualenv ~/.virtualenv-3.9.9/django-4.0
    . ~/.virtualenv-3.9.9/django-4.0/bin/activate
    pip install django=='4.0.*'
    git checkout https://github.com/seguri/django-polls-tutorial
    cd django-polls-tutorial
    git checkout -b django-4.0
    python manage.py migrate
    python manage.py createsuperuser
    python manage.py runserver

# After

    . ~/.virtualenv-3.6.1/django-2.1/bin/activate
    python manage.py runserver

