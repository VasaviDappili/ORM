# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![alt text](<Screenshot 2024-02-29 141259-1.png>)

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
```
```
admin.py
from django.contrib import admin
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)
```
## OUTPUT

#![alt text](<Screenshot 2024-02-27 160741.png>)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
