# Meta Back-End Developer Capstone

![Coursera](https://img.shields.io/badge/Coursera-0747a6?style=flat&logo=coursera&logoColor=white)
![Meta](https://img.shields.io/badge/Meta-0668E1?style=flat&logo=meta&logoColor=white)
![Django](https://img.shields.io/badge/Django-092e20?style=flat&logo=django&logoColor=white)

Building RESTful APIs using [Django Rest Framework](https://www.django-rest-framework.org/) connected to a [MySQL](https://dev.mysql.com/downloads/) as part of the [Meta Back-End Developer Certificate](https://www.coursera.org/professional-certificates/meta-back-end-developer) teached by [Meta](https://www.facebook.com/business/learn/back-end-back-end-developer-certificate-coursera).

<p align="center">
    <a href="https://www.credly.com/org/facebook-blueprint/badge/meta-back-end-developer-certificate">
        <img src="images/meta-backend-cert.png" width="30%" height="30%" />
    </a>
</p>

## Grading criteria

* Is the capstone project setup correctly? Does it contain a project called `littlelemon` and an app called `restaurant`? :white_check_mark:
* Open `settings.py`. Does the `INSTALLED_APPS` list contain the name of the app `restaurant`, `rest_framework`, and `djoser`? :white_check_mark:
* In `settings.py` does the `TEMPLATES` section contain the `DIRS` attribute set to templates? :white_check_mark:
* Does the capstone project contain an `index.html` file, it's associated view and has the URL routing been setup successfully? :white_check_mark:
* Does the capstone project contain a MySQL database and is it setup correctly inside the DATABASES section in the settings.py file? :white_check_mark:
* Open the file `models.py`. Does this file contain the code for the models `Menu` and `Booking`? :white_check_mark:
* Have the models been registered in the file `admin.py`? :white_check_mark:
* Open `serializers.py`. Does it contain the code for Serializer classes for the `Menu` and `Booking` models? :white_check_mark:
* Open `views.py`. Does it contain the code for viewset classes of for the Menu and Booking models? :white_check_mark:
* Open the `urls.py` file of the app, does it contain the `api-token-auth` route that invokes the `obtain_auth_token` view? :white_check_mark:
* Open the `urls.py` file of the project, does it contain the code for the `djoser` endpoints? :white_check_mark:
* Can you test the API by visiting the API endpoints provided by the learner using a using browsable API? :white_check_mark:
* Does the capstone project contain files called `test_views.py` and `test_models.py`. Does this file contain the unit test code? :white_check_mark:
* Can you test the project using the Insomnia client app? :white_check_mark:

## Steps to run the app

### 1. Install `pipenv`

```bash
pip install pipenv
```

### 2. Create a `.env` file in the root folder

```bash
# .env
DATABASE = YOUR_MYSQL_DATABASE_NAME
USER     = YOUR_USERNAME             # default is root
PASSWORD = YOUR_MYSQL_PASSWORD
HOST     = localhost                 # or 127.0.0.1
PORT     = 3306
```

### 3. Install dependencies

```bash
pipenv install
```

### 4. Make migrations

```bash
py manage.py makemigrations
```

### 5. Migrate

```bash
py manage.py migrate
```

### 6. Run the app

```bash
py manage.py runserver
```

### To run tests

```bash
py manage.py test tests
```
