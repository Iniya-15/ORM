# Ex02 Django ORM Web Application
## Date: 1.05.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## ER Diagram

![Screenshot 2025-05-01 205928](https://github.com/user-attachments/assets/ad10d9a1-f0ed-4586-b82c-68b668670450)

## PROGRAM
```
admin.py

from django.contrib import admin
from .models import Employee, EmployeeAdmin

admin.site.register(Employee, EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin

class Employee(models.Model):
    eid = models.CharField(max_length=20, help_text="Employee ID")
    name = models.CharField(max_length=100)
    salary = models.IntegerField()
    age = models.IntegerField()
    email = models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display = ('eid', 'name', 'salary', 'age', 'email')
```


## OUTPUT

![Screenshot 2025-05-01 031159](https://github.com/user-attachments/assets/7c95bfbe-b8cf-4eaa-ae5a-2200fbb94cc4)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
