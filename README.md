# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![Entity Relationship Diagram](./Ex02_ORM.png)

## DESIGN STEPS


### STEP 1:
Change the URL of the GitHub remote repository

### STEP 2:
Push the changes in the branch to the Github repository

### STEP 3:
Create a migration file that contains code for the database schema of a model


## PROGRAM
```
admin.py
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py
from django.db import models
from django.contrib import admin
class Employee(models.Model):
    eid=models.CharField(max_length=100)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```


## OUTPUT
![OUTPUT](./EX02.png)

## RESULT
The program executed successfully