# Ex02 Django ORM Web Application

NAME : PRIYANKA K

DEPARTMENT : ARTIFICIAL INTELLIGENCE AND DATA SCIENCE

REGISTER NO. : 212223230162

## Date: 

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub.

### STEP 2:
Create a new app in Django project.

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players.

## PROGRAM:
```
# Register your models here.
from django.contrib import admin
from .models import footballPlayer,footballPlayerAdmin
admin.site.register(footballPlayer,footballPlayerAdmin)
```
```
# Create your models here.
from django.db import models
from django.contrib import admin
class footballPlayer(models.Model):
	name=models.CharField(max_length=30)
	age=models.IntegerField()
	goals=models.IntegerField()
	jerseynumber=models.IntegerField()
	team=models.CharField(max_length=25)
	NumberofMatches=models.IntegerField()
class footballPlayerAdmin(admin.ModelAdmin):
	list_display=["name","age","goals","jerseynumber","team","NumberofMatches"]
```

## OUTPUT:

![image](https://github.com/Priyanka1846/ORM/assets/139425809/cb884d97-e795-4240-afdd-54f86e1ef088)

## RESULT:
Thus the program for creating a database using ORM hass been executed successfully.
