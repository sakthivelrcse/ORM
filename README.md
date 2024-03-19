# Ex02 Django ORM Web Application
## Date: 15-03-2024

## AIM
To develop a Django application to store and retrieve data from a railway database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![erp diagram](https://github.com/sakthivelrcse/ORM/assets/116993934/629b0600-7c1e-413d-8c54-21826c13c99a)


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
admin.py

from django.contrib import admin
from .models import railway,railwayAdmin
admin.site.register(railway,railwayAdmin)

models.py

from django.db import models
from django.contrib import admin
class railway (models.Model):
    train_code=models.CharField(max_length=20,help_text="railway train_code")
    train_name=models.CharField(max_length=100)
    start_time=models.IntegerField()
    End_time=models.IntegerField()
    start_station_code=models.IntegerField()
    end_station_code=models.IntegerField()
    
 
class railwayAdmin(admin.ModelAdmin):
    list_display=('train_code','train_name','start_time','End_time','start_station_code','end_station_code',)
```
## OUTPUT

![Screenshot 2024-03-13 155527](https://github.com/sakthivelrcse/ORM/assets/116993934/7cc564d4-a90d-445e-9c87-26234f4658cb)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
