# CS178A-B-Template

## Table of Contents
- [Overview](#overview)
- [Usage](#usage)
- [How To Run](#how-to-run)
- [Diagrams](#diagrams)
- [Dependencies](#dependencies)
- [Description](#Description)

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
python manage.py runserver localhost:8000
```
In the Browser visit: [http://127.0.0.1:8000/](http://localhost:3000/)


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

## Description
    
As a programmer, it is natural to deal with code every day, and inevitably encounter various problems and various bugs, which requires timely recording of problems and methods to solve them, both for themselves and others. However, many programmers do not like to write things. I have been studying computer for nearly a year, so far, I still often think of my cousin who said that if you don't solve 1000 problems, you are not a beginner in this industry... Look up to some god-level programmers such as Wu Hanqing, Lou Tiancheng, Ruan Yifeng , Liao Xuefeng, his personal blog has been built, maintained and updated for many years. So we follow the example of various great gods and build a personal blog system as the first simple and small project of our group web development.
After we collect various articles and analyze their value, we import them into our group blog system, and after setting tags in the background, the system automatically categorizes them and provides keyword search function. After categorizing, you can refer to the articles according to your personal preferences. Due to time and technical reasons, this blog is version 1.0, and our team will add scrapy crawler for article crawling and server deployment in the future.
    
 The main functions:
  1. Search engine
  2. Classification and filing
  3. Review the application
  4. Statistics of reading volume and number of articles
  5. Page sidebar and tag cloud
  6. Background management
