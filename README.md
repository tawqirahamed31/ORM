# Ex01 Django ORM Web Application
## Date: 
3-12-2025
## AIM
To develop a Django Application to store and retrieve data from a E-Commerce Website Database for Amazon or Flipkart using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
<img width="679" height="385" alt="image" src="https://github.com/user-attachments/assets/7b66a19e-f2d4-43d0-8061-84c1e9b389f0" />



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

    class car(models.Model):
        vin = models.CharField(max_length=20, unique=True)
        make = models.CharField(max_length=50)
        model = models.CharField(max_length=50)
        year = models.IntegerField()
        price = models.DecimalField(max_digits=12, decimal_places=2)
        mileage = models.IntegerField(max_length=30)
        color = models.CharField(max_length=30)
        available = models.BooleanField(default=True)
        created_at = models.DateTimeField(auto_now_add=True)

    def __str__(self):
        return f"{self.make}{self.model}({self.year})"

## OUTPUT
<img width="1919" height="946" alt="image" src="https://github.com/user-attachments/assets/066e064d-d598-4821-b722-e77584523300" />



## RESULT
Thus the program for creating E-commerce website database using ORM hass been executed successfully
