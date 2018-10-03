# django-polls-tutorial

This is the solution code to the [Django official tutorial](https://docs.djangoproject.com/en/2.1/intro/tutorial01/), using:

    $ python --version && echo -n 'Django ' && python -m django --version
    Python 3.6.1
    Django 2.1.2

# First time

    mkdir ~/.virtualenv-3.6.1
    virtualenv ~/.virtualenv-3.6.1/django-2.1
    . ~/.virtualenv-3.6.1/django-2.1/bin/activate
    pip install django=='2.1.*'
    git checkout https://github.com/seguri/django-polls-tutorial
    cd django-polls-tutorial
    git checkout -b django-2.1
    python manage.py migrate
    python manage.py createsuperuser
    python manage.py runserver

# After

    . ~/.virtualenv-3.6.1/django-2.1/bin/activate
    python manage.py runserver

