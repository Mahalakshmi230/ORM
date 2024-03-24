# Ex02 Django ORM Web Application
## Date:7/2/24 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/Mahalakshmi230/ORM/assets/149365324/aadb5f42-92e0-4db0-a229-c10e6aadb856)


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
admin.py

from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)

models.py

from django.db import models
from django.contrib import admin
class Book(models.Model):
   serialno=models.IntegerField(primary_key=True);
   Bookname=models.CharField(max_length=30);
   Author=models.CharField(max_length=20);
   publishedDate=models.DateField();
   Booktype=models.CharField(max_length=20);
class BookAdmin(admin.ModelAdmin):
   list_display=("serialno","Bookname","Author","publishedDate","Booktype");

```

## OUTPUT
![Screenshot 2024-03-24 210232](https://github.com/Mahalakshmi230/ORM/assets/149365324/7e90f839-87d2-4e7b-a974-2feedb9cee4f)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
