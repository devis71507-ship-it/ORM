# Ex02 Django ORM Web Application
## Date: 08/10/2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
```
from django.db import models
from django.contrib import admin
class Car2(models.Model):
    car_name = models.CharField()
    car_model = models.CharField()
    release_date = models.DateField()
    millage = models.IntegerField()
    colour = models.CharField()

class Car2Admin(admin.ModelAdmin):
    list_display = ('car_name', 'car_model', 'release_date', 'millage', 'colour')
from django.contrib import admin
from.models import Car2,Car2Admin
admin.site.register(Car2,Car2Admin)
```



## OUTPUT

![alt text](<Screenshot 2025-10-08 134654.png>)


## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
