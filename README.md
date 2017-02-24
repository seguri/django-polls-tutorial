# django-polls-tutorial

This is the solution code to the [Django official tutorial](https://github.com/Chive/django-poll-app), using:

    $ python --version && echo -n 'Django ' && python -m django --version
    Python 3.4.5
    Django 1.10.5

I made it as a quick way to clone a working Django app.

The idea is to have a branch for each version of Django but I won't promise I'll actually do it 😛

# First time

    mkdir ~/.virtualenv-3.4.5
    virtualenv ~/.virtualenv-3.4.5/django-1.10
    . ~/.virtualenv-3.4.5/django-1.10/bin/activate
    pip install django==1.10.5
    git checkout https://github.com/seguri/django-polls-tutorial
    cd django-polls-tutorial
    git checkout -b django-1.10 remotes/origin/django-1.10
    python manage.py migrate
    python manage.py createsuperuser
    python manage.py runserver

# After

    . ~/.virtualenv-3.4.5/django-1.10/bin/activate
    python manage.py runserver

# Notes

How I renamed the remote branch, thanks to [SO](http://stackoverflow.com/a/4754132/1521064):

    git checkout https://github.com/seguri/django-polls-tutorial
    cd django-polls-tutorial
    git checkout -b django-1.10.5 remotes/origin/django-1.10.5 # This probably isn't neccesary
    git branch django-1.10 origin/django-1.10.5
    git push origin --set-upstream django-1.10
    git push origin :django-1.10.5

