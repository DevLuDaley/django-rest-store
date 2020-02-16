sidecar-django-rest-store

# create env

python3 -m venv venv_django_rest_store

# activate env

source venv_django_rest_store/bin/activate

# install django

# 'Installing collected packages: asgiref, sqlparse, pytz, django'

# WARNING: You are using pip version 19.2.3, however version 20.0.2 is available.

# You should consider upgrading via the 'pip install --upgrade pip' command.

pip install django

-
pip install djangorestframework

-
pip install django-filter

# add 'django_filters' to your INSTALLED_APPS.

-
pip install pillow

# add '127.0.0.1' to allowed_hosts in setttings.py

-
pip install mock==0.8.0
