# Ex02 Django ORM Web Application
## Date: 04.04.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

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
Execute Django admin and create details for 10 books

## PROGRAM
admin.py

from django.contrib import admin
from .models import football_players,football_playersAdmin
admin.site.register(football_players,football_playersAdmin)

models.py

from django.db import models
from django.contrib import admin
class football_players(models.Model):
  first_name=models.CharField(max_length=30)
  last_name=models.CharField(max_length=30)
  dob=models.DateField()
  age=models.IntegerField()
  matches_played=models.IntegerField()
  total_goals=models.IntegerField()
  email=models.EmailField()

class football_playersAdmin(admin.ModelAdmin):
  list_display=('first_name','last_name','dob','age','matches_played','total_goals','email')
## OUTPUT

![Screenshot (29)](https://github.com/BharathJayachandran/ORM/assets/122089525/9da38c67-b4c0-4b9a-b8be-a19a05471591)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
