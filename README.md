# Ex02 Django ORM Web Application
## Date:22/11/26

## AIM
To develop a Django Application to store and retrieve data from a Vehicle Service Database platform using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM

```

from django.db import models

class FoodItem(models.Model):
    food_id = models.AutoField(primary_key=True)
    food_name = models.CharField(max_length=100)
    restaurant_name = models.CharField(max_length=100)
    category = models.CharField(max_length=50)
    price = models.IntegerField()
    rating = models.FloatField()
    availability = models.BooleanField(default=True)

    class Meta:
        db_table = 'food_details'

    def __str__(self):
        return self.food_name

```

## OUTPUT

<img width="1515" height="763" alt="image" src="https://github.com/user-attachments/assets/958813ef-2bc0-49c3-8243-ec8e27ceb7c1" />


## RESULT
Thus the program for creating vehicle service Database using ORM hss been executed successfully.
