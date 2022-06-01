# CS178A-B-Template

## Table of Contents
- [Overview](#overview)
- [Usage](#usage)
- [How To Run](#how-to-run)
- [Diagrams](#diagrams)
- [Dependencies](#dependencies)

## Overview
<Include project description?

## Team
<a href="https://github.com/msalloum" target="_blank"><img src="https://avatars3.githubusercontent.com/u/1790819?s=400&v=4" align="left" height="30px">Mariam Salloum </a>

## Usage
Demo: <Link to youtube video>

<Screenshot of application>

## How To Run
In the project directory find the blogproject/settings.py, and modify this file for your MySQL server(default is my account and password).
```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'HOST':'localhost',
        'PORT':'3306',
        'USER':'admin',
        'PASSWORD':'Admin!123456',
        'NAME': 'blogdb',
    }
}
```
Create the DataBase
In the terminal we should migrate the database files for Django:
```bash
python manage.py makemigrations
python manage.py migrate
```
Create the SuperUser

In the terminal we should create a SuperUser as manager to operate Blog in the backstage of Django
```bash
python manage.py createsuperuser
```
Start Running
Execute: 
 ```bash
python manage.py runserver
```
In the Browser visit: http://127.0.0.1:8000/


## Diagrams

Sequence Diagram

Frontend Structure


Overall System Diagram

## Dependencies
Using the Python's Django framework as backend server and frontend is static HTML+JS+CSS. 
Easily install the packages needed: 
```bash
 pip install requirements.txt 
```
    
If you don't have pip, 

    OS X / Linux, in the terminal run:

    curl http://peak.telecommunity.com/dist/ez_setup.py | python
    curl https://bootstrap.pypa.io/get-pip.py | python

    Windows:

    http://peak.telecommunity.com/dist/ez_setup.py and https://raw.github.com/pypa/pip/master/contrib/get-pip.py 


