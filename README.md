# Django Blog

## Demo


## About

The blog was created while learning from Maximilian Schwarzmüller's Course on Udemy.      
https://www.udemy.com/course/python-django-the-practical-guide/    

The course deals with topics such as:
- Basics of Django (MTV, Admin panel, Forms and so on...)
- Class Views & Generic Views
- Sessions
- Deployment on AWS

The project is actually rewritten, but sometimes I used my own inventions :)



## Setup


- ``` git clone https://github.com/kurekhombre/photobucket.git ```
- Create virtual environment ```python3 -m venv venv``` and activate it
  - Linux/Mac ``` source venv/bin/activate ```
  - Windows ``` venv\Scripts\activate.bat ```
- ``` pip install -r requirements.text ```
- Generate SECRET KEY with 
  - https://djecrety.ir/ or 
  - ``` python manage.py shell ``` 
   ``` >>> from django.core.management.utils import get_random_secret_key``` 
  ``` print(get_random_secret_key) ```
- Create  file '.env' in project folder and paste ``` SECRET_KEY='<your_key>' ```
- ``` python manage.py makemigrations ```
- ``` python manage.py migrate ```
- ``` python manage.py runserver ```