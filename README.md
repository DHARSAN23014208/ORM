# Ex02 Django ORM Web Application
## Date: 21.04.2025
# NAME: DHARSAN KUMAR R
# REG:212223240028
## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM


![ER](https://github.com/user-attachments/assets/41de3e05-436e-4fc5-8e79-b72958b07745)

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
from .models import Movies,MoviesAdmin
admin.site.register(Movies,MoviesAdmin)


models.py

from django.db import models
from django.contrib import admin
class Movies(models.Model):
    userid=models.IntegerField(primary_key=True)
    username=models.CharField(max_length=30)
    mobileno=models.IntegerField()
    mailid=models.EmailField()
    moviename=models.CharField(max_length=50)
    noofseats=models.IntegerField()
    date=models.DateField()

class MoviesAdmin(admin.ModelAdmin):
    list_display=('username','moviename','noofseats','mailid')
```
## OUTPUT

![Screenshot 2025-04-11 203923](https://github.com/user-attachments/assets/df74d500-616c-4f2b-bf0d-ff6caaa638cf)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
