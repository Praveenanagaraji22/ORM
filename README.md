# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![primary](https://user-images.githubusercontent.com/119393514/215305090-76f4f37b-6059-480f-8d74-61ae6b64028b.jpeg)


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
![orm](https://user-images.githubusercontent.com/119393514/215305023-9722c722-8376-418e-8ee2-099ebc4e2289.jpeg)


## RESULT
The program executed successfully
