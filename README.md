# recipe-app-api
Recipe app api source code

# To build the image specified in the Dockerfile

docker build .

# To compose the docker

docker-compose build

# To start the django project

docker-compose run app sh -c "django-admin.py startproject app ."

# To run the test 

docker-compose run app sh -c "python manage.py test && flake8"

# To create an app in the project

docker-compose run app sh -c "python manage.py startapp {appname}"