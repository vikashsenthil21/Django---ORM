# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![no](ormdiagram.png)



## DESIGN STEPS

### STEP 1:
creaste and collect the information from customer using django applications.

### STEP 2:
Type the code in python

### STEP 3:
Push into github


## PROGRAM
```
admin.py:

from django.contrib import admin
from .models import Studentdetail,StudentdetailAdmin


admin.site.register(Studentdetail,StudentdetailAdmin)
```
```
from django.db import models

# Create your models here. 
from django.db import models
from django.contrib import admin
# Create your models here.
class Customer(models.Model):
    customerid = models.CharField(max_length=8,primary_key=True)
    customername =models.CharField(max_length=100)
    mobilenumber =models.CharField(max_length=100)
    email = models.EmailField()
    quantity= models.IntegerField()
    

class CustomerAdmin(admin.ModelAdmin):
    list_display = ('customerid','customername','mobilenumber','email','quantity')
```

## OUTPUT

![nothing](orm.png)


## RESULT
Thus the experiment was executed successfully..
