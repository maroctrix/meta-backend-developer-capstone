<p align="center">
    <a href="https://www.credly.com/org/facebook-blueprint/badge/meta-back-end-developer-certificate">
        <img src="images/meta-backend-cert.png" width="30%" height="30%" />
    </a>
</p>

<h1 align="center">Meta Back-End Developer Capstone</h1>

<p align="center">
    <img src="https://img.shields.io/badge/Coursera-0747a6?style=flat&logo=coursera&logoColor=white" />
    <img src="https://img.shields.io/badge/Meta-e2e2e2?style=flat&logo=meta&logoColor=0668E1" />
    <img src="https://img.shields.io/badge/Django-092e20?style=flat&logo=django&logoColor=white" />
    <img src="https://img.shields.io/badge/Grading%20criteria-Passing-brightgreen" />
</p>


## Description
This is the capstone project of [Meta Back-End Developer Certificate](https://www.coursera.org/professional-certificates/meta-back-end-developer) teached by [Meta](https://www.facebook.com/business/learn/back-end-back-end-developer-certificate-coursera) which includes the following courses:

* [Introduction to Back-End Development](https://www.coursera.org/learn/introduction-to-back-end-development?specialization=meta-back-end-developer)
* [Programming in Python](https://www.coursera.org/learn/programming-in-python?specialization=meta-back-end-developer)
* [Version Control](https://www.coursera.org/learn/introduction-to-version-control?specialization=meta-back-end-developer)
* [Introduction to Databases for Back-End Development](https://www.coursera.org/learn/intro-to-databases-back-end-development?specialization=meta-back-end-developer)
* [Django Web Framework](https://www.coursera.org/learn/django-web-framework?specialization=meta-back-end-developer)
* [APIs](https://www.coursera.org/learn/apis?specialization=meta-back-end-developer)
* [The Full Stack](https://www.coursera.org/learn/the-full-stack?specialization=meta-back-end-developer)
* [Back-End Developer Capstone](https://www.coursera.org/learn/back-end-developer-capstone?specialization=meta-back-end-developer)
* [Coding Interview Preparation](https://www.coursera.org/learn/coding-interview-preparation?specialization=meta-back-end-developer)

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
