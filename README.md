# django-polls-tutorial

This is the solution code to the [Django official tutorial](https://docs.djangoproject.com/en/1.11/intro/tutorial01/), using:

    $ python --version && echo -n 'Django ' && python -m django --version
    Python 3.4.5
    Django 1.11

I made it as a quick way to clone a working Django app.

The idea is to have a branch for each version of Django but I won't promise I'll actually do it 😛

# First time

    mkdir ~/.virtualenv-3.4.5
    virtualenv ~/.virtualenv-3.4.5/django-1.11
    . ~/.virtualenv-3.4.5/django-1.11/bin/activate
    pip install django==1.11
    git checkout https://github.com/seguri/django-polls-tutorial
    cd django-polls-tutorial
    git checkout -b django-1.11 remotes/origin/django-1.11
    python manage.py migrate
    python manage.py createsuperuser
    python manage.py runserver

# After

    . ~/.virtualenv-3.4.5/django-1.11/bin/activate
    python manage.py runserver

