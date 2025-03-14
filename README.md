# Ex02 Django ORM Web Application
## Date: 10/10/23

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
# models.py
```
from django.db import models
from django.contrib import admin
class Football (models.Model):
    jerseyno=models.CharField(max_length=20,help_text="jerseyno")
    name=models.CharField(max_length=100)
    country=models.CharField(max_length=50)
    age=models.IntegerField()
    YOE=models.IntegerField()

class FootballAdmin(admin.ModelAdmin):
    list_display=('jerseyno','name','country','age','YOE')
```
# admin.py
```
from django.contrib import admin
from .models import Football,FootballAdmin
admin.site.register(Football,FootballAdmin)
```



## OUTPUT

![image](https://github.com/Irenejecinthamerlin/ORM/assets/128350225/ce7f8c95-99b4-4743-9bf0-30bfbe59975a)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
