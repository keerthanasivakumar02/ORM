# Ex02 Django ORM Web Application
## Date: 29-02-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![Screenshot 2024-02-29 142548](https://github.com/keerthanasivakumar02/ORM/assets/150827397/e18c65e7-9572-4e52-a507-0d8672704414)


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
class Book(models.Model):
   title=models.CharField(max_length=30);
   year_of_publishing=models.DateField(); 
   author_name=models.CharField(max_length=20);
   no_of_pages=models.IntegerField();
   book_price=models.IntegerField();
class BookAdmin(admin.ModelAdmin):
   list_display=("title","year_of_publishing","author_name","no_of_pages","book_price");    

admin.py
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)


```

## OUTPUT

![ormapp](https://github.com/keerthanasivakumar02/ORM/assets/150827397/a5e5384a-403f-49e3-859b-d3fdf69fc913)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
