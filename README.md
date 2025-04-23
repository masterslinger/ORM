# Ex02 Django ORM Web Application
## Date: 23/04/2025

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/8b6facfc-303f-45c0-ad12-cd8733a0d3eb)


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
models.py

from django.db import models
from django.contrib import admin
class customer (models.Model):
    c_id=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class customerAdmin(admin.ModelAdmin):
    list_display=('c_id','name','salary','age','email')
 
admin.py

from django.contrib import admin
from .models import customer,customerAdmin
admin.site.register(customer,customerAdmin)
```

## OUTPUT

![image](https://github.com/user-attachments/assets/a1bba0f1-19bb-48ac-9366-80b7c9189e9f)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
