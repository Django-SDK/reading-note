# Class 4 Quiz


## 1. how to create a Django project?
  <!-- 

```bash
django-admin startproject mysite
```
-->

## 2. how to create a Django app?
  <!-- 

```bash
python manage.py startapp myapp
```
-->

## 3. how to create a Django view?
  <!-- 

```python
from django.http import HttpResponse

def index(request):
    return HttpResponse("Hello, world. You're at the polls index.")
```

-->

## 4. how to create a Django URL?
  <!-- 

```python
from django.urls import path


from . import views

urlpatterns = [
    path('', views.index, name='index'),
]
```
-->

## 5. how to create a Django template?
  <!-- 

```html
{% extends "base_generic.html" %}

{% block content %}
    <h1>My Polls</h1>
    <ul>
    {% for poll in latest_poll_list %}
        <li><a href="{% url 'polls:detail' poll.id %}">{{ poll.question }}</a></li>
    {% endfor %}
    </ul>
{% endblock %}
```
-->

