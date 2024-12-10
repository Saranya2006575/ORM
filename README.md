# Ex02 Django ORM Web Application
# Date:10.10.24
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
```
admin.py

from django.contrib import admin
from .models import Customer,CustomerAdmin
admin.site.register(Customer,CustomerAdmin)

models.py

from django.db import models
from django.contrib import admin
class Customer(models.Model):
     Name=models.CharField(max_length=10)
     Accno=models.IntegerField(primary_key="accno")
     Email=models.EmailField()
     Dob=models.DateField()
     Adharno=models.IntegerField()

class CustomerAdmin(admin.ModelAdmin):
     list_display=('Name','Accno','Email','Dob','Adharno')

```
# OUTPUT
![Screenshot 2024-12-10 220426](https://github.com/user-attachments/assets/a9666b6b-47c6-4bfc-b084-3eab720a94ca)


# RESULT
Thus the program for creating a database using ORM hass been executed successfully
