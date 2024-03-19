# Ex02 Django ORM Web Application
## Date: 19/03/2024

## AIM
To develop a Django application to store and retrieve data from a Railway database using Object Relational Mapping(ORM).
## Entity Relationship Diagram
![Screenshot 2024-03-12 205556](https://github.com/BhumireddyLakshmivardhanreddy/ORM/assets/148514637/7bbda771-b87c-4098-836f-e214e58980fa)

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
from .models import Train, TrainAdmin
admin.site.register(Train,TrainAdmin)

models.py
from django.db import models
from django.contrib import admin
class Train(models.Model):
    Train_code=models.CharField(max_length=20,primary_key=True)
    Train_name=models.CharField(max_length=100)
    start_time=models.DateTimeField()
    End_time=models.DateTimeField()
    start_station_code=models.CharField(max_length=20)
    End_station_code=models.CharField(max_length=20)
 
class TrainAdmin(admin.ModelAdmin):
    list_display=('Train_code','Train_name','start_time','End_time','start_station_code','End_station_code')
```

## OUTPUT

![WhatsApp Image 2024-03-19 at 11 08 19_a852f225](https://github.com/BhumireddyLakshmivardhanreddy/ORM/assets/148514637/1f63faf8-a556-4d1c-9d87-111179bbcaae)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
