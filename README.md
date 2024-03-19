# Ex02 Django ORM Web Application
## Date: 15-03-2024

## AIM
To develop a Django application to store and retrieve data from a railway database using Object Relational Mapping(ORM).

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
Execute Django admin and create details for 10 records

## PROGRAM
```
model.py

from django.db import models
from django.contrib import admin
class Railway_db(models.Model):
    trainno=models.IntegerField(primary_key=True);
    trainname=models.CharField(max_length=20);
    departure=models.CharField(max_length=50);
    arrival=models.CharField(max_length=50);
    distance=models.IntegerField();
class Railway_dbAdmin(admin.ModelAdmin):
    list_display=("trainno","trainname","departure","arrival","distance");

admin.py

from django.contrib import admin
from .models import Railway_db,Railway_dbAdmin
admin.site.register(Railway_db,Railway_dbAdmin
```
## OUTPUT
![WhatsApp Image 2024-03-19 at 10 49 59 AM](https://github.com/sakthivelrcse/ORM/assets/116993934/1fd9fe7f-3f5e-4daa-982e-b3e727ddbd9c)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
