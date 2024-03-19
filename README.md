# Ex02 Django ORM Web Application
## Date: 15-03-2024

## AIM
To develop a Django application to store and retrieve data from a railway database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![erp diagram ](https://github.com/sakthivelrcse/ORM/assets/116993934/bf47f13e-e7b3-4d29-93b0-356a92799083)



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
    train_code=models.CharField(max_length=20,help_text="railway train_code")(primary_key=True)
    train_name=models.CharField(max_length=100)
    start_time=models.IntegerField()
    End_time=models.IntegerField()
    start_station_code=models.IntegerField()
    end_station_code=models.IntegerField()
    
 
class railwayAdmin(admin.ModelAdmin):
    list_display=('train_code','train_name','start_time','End_time','start_station_code','end_station_code',)
```
## OUTPUT

![Screenshot 2024-03-15 091508](https://github.com/sakthivelrcse/ORM/assets/116993934/4e806555-2430-4ab7-a99e-2da516ce89af)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
