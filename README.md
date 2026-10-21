# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django Application to store and retrieve data from a Vehicle Service Database platform using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
admin.py
'''
from django.contrib import admin
from .models import FoodItem

admin.site.register(FoodItem)
'''
'''
models.py

'''from django.db import models

class FoodItem(models.Model):
    name = models.CharField(max_length=100)
    restaurant = models.CharField(max_length=100)
    price = models.DecimalField(max_digits=8, decimal_places=2)
    category = models.CharField(max_length=50)
    is_available = models.BooleanField(default=True)

    def __str__(self):
        return self.name

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM



## OUTPUT
![alt text](<Screenshot 2026-10-15 214543.png>)


## RESULT
Thus the program for creating vehicle service Database using ORM hss been executed successfully.
