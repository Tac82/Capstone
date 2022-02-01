# Kreations

## Overview

* Blog-like application, similar to market websites such as offerup, craigslist, letgo, ect. It will allow one admin user to upload an image, description, price and a catagory to that product.
* The one and only account registered to the application will be an admin. They should be able to edit and delete an item that has already been posted. 
* Clients/customers who visit the applications website should be directed to a homepage with the websites' logo. Interacting with the navbars' search bar or dropdown menu of pre-determined categories should direct the client to their requested search. 
* Items that have been posted will be showcased in a url dedicated to their category.
* Clients who find item(s) they want to order will have to click on the a button in the navbar that directs them to a contact page. This should have the admin's contact information.


## Functionality
Searching for products/items will be available to unathenticated users, as they can't make an account anyways. However the admin account will need it.
When the admin account wants to post a product, it will instantiate a Products and Categories model with form data.


## Data Model
Product
* author, foreignKey(user)
* category, ManyToManyField('name')
* image, models.ImageField()
* title, forms.CharField()
* price, models.PositiveIntegerField()
* description, forms.CharField()
* created_date, forms.DateField()

Categories
* name, forms.CharField()

## Schedule
- Week 1
  - Rough landing page, superuser login page and another page for a basic form to send data into product models.

- Week 2
  - Category pages working with products appearing in them. Allow the superuser to edit and delete posts. Possibly fit the search bar functionality into this week.

- Week 3
  - Front-end work, style it up and fix layouts.

- Week 4
  - Stress test the application, fill it with lots of data. If it looks too clunky and unorganized with lots of products, implement page functions for items.
