# Ex01 Django ORM Web Application
## Date: 19/12/25

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
class Car_DB(models.Model):
	Car_name=models.CharField(max_length=20)
	Fuel_efficient=models.FloatField()
	Color=models.CharField(max_length=10)
	Price=models.IntegerField()
	CarID=models.IntegerField(primary_key=True)
class Car_DBAdmin(admin.ModelAdmin):
	list_display=["Car_name","Fuel_efficient","Color","Price","CarID"]
```

admin.py

from django.contrib import admin
from .models import Car_DB,Car_DBAdmin
admin.site.register(Car_DB,Car_DBAdmin)


## OUTPUT
<img width="1044" height="607" alt="image" src="https://github.com/user-attachments/assets/ac8202ec-b92d-4bd4-b136-e56042b4d23b" />



## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
