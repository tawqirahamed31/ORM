# Ex01 Django ORM Web Application
## Date: 
3-12-2025
## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

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
    from django.db import models
    from django.contrib import admin
    class Employee (models.Model):
        eid=models.CharField(max_length=20,primary_key="eid")
        name=models.CharField(max_length=100)
        salary=models.IntegerField()
        age=models.IntegerField()
        email=models.EmailField()
 
    class EmployeeAdmin(admin.ModelAdmin):
        list_display=('eid','name','salary','age','email')
## OUTPUT
<img width="1919" height="988" alt="image" src="https://github.com/user-attachments/assets/cc689efc-82b7-48aa-902b-d5b54f924c23" />




## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
