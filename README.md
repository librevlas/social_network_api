# Social Network API

This is simple REST API written in Python.


## Stack
- Python3
- [Django](https://www.djangoproject.com/)
- [Django REST Framework](https://www.django-rest-framework.org/)
- [Djoser](https://djoser.readthedocs.io/en/latest/)
- [Simple JWT](https://django-rest-framework-simplejwt.readthedocs.io/en/latest/)


## Features
- User create/login/signup
- Post create
- Post like/unlike
- Analytics about how many likes was made (use date_from and date_to parametrs to filter date)
- Endpoint with user activity information (last login and last seen time)


## Usage
Action | URL | Method
------------ | ------------- | -------------
Create user | /api/v1/auth/users/ | POST
User activity | /api/v1/auth/activity/ | GET
Obtain token | /api/v1/auth/token/ | POST
Refresh token | /api/v1/auth/refresh/ | POST
Create post | /api/v1/posts/ | POST 
List of posts | /api/v1/posts/ | GET
Get post | /api/v1/posts/<int:pk> | GET 
Like post | /api/v1/posts/<int:pk>/like/ | POST
Unlike post | /api/v1/posts/<int:pk>/unlike/ | POST
Like analytics | /api/v1/analytics/ | GET

