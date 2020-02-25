sidecar-django-rest-store

# create env

python3 -m venv venv_django_rest_store

# activate env

source venv_django_rest_store/bin/activate

# install django

pip install django

-

* 'Installing collected packages: asgiref, sqlparse, pytz, django'
* WARNING: You are using pip version 19.2.3, however version 20.0.2 is available.
* You should consider upgrading via the 'pip install --upgrade pip' command.

-

-

pip install djangorestframework

-
pip install django-filter

# add 'django_filters' to your INSTALLED_APPS.

-
pip install pillow

# add '127.0.0.1' to allowed_hosts in setttings.py

-
▶ pip install mock==0.8.0

-
▶ python3 manage.py makemigrations

▶ python3 manage.py migrate

- Operations to perform:
- Apply all migrations: admin, auth, contenttypes, sessions, store
- Running migrations:
- Applying auth.0010_alter_group_name_max_length... OK
- Applying auth.0011_update_proxy_permissions... OK

# access the db using the python shell

▶ ./manage.py shell

# import modules

> > > from store.models import Product
> > > product = Product.objects.all()[0]
> > > from store.serializers import ProductSerializer
> > > serializer = ProductSerializer()
> > > data = serializer.to_representation(product)
> > > from rest_framework.renderers import JSONRenderer
> > > renderer = JSONRenderer()
> > > print(renderer.render(data))

-         b'{
              "id":1,
              "name":"Mineral Water Strawberry!",
              "description":"Natural-flavored strawberry with an anti-oxidant kick.","price":1.0,"sale_start":null,"sale_end":null,"is_on_sale":false,"current_price":1.0}'
-
