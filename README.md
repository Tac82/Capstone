# Kreations

## Overview

* Blog-like application, similar to market websites such as offerup, craigslist, letgo, ect. It will allow one admin user to upload an image, description, price, catagory and a subcategory to that post.
* The one and only account registered to the application will be an admin. They should be able to edit and delete an item that has already been posted. 
* Clients/customers who visit the applications website should be directed to a homepage with the websites' logo. Interacting with the navbars' search bar or dropdown menu of pre-determined categories should direct the client to their requested search or subcatagories. 
* Items that have been posted will be showcased in their dedicated category url underneath the subcategory it is tagged with. 
* Clients who find item(s) they want to order will have to click on the a button in the navbar that directs them to a contact page. This should have the admin's contact information.


## Functionality
Searching for posts/items will be available to unathenticated users, as they can't make an account anyways. However the admin account will need it.
When the admin account wants to make a post, it will instantiate a Posts model with form data.

Categories and subcategories work as such. Drop down menu showcases catagories, each with their own url. Once directed to a url, the items will be in a column of their assigned subcategory. For example, women's shoes are in a category of women's clothing, and the shoes will be listed as 'shoes' in the subcategory. 

## Data Model
Posts
* image, models.ImageField()
* title, forms.CharField()
* description, forms.CharField()
* category, forms.CharField()
* subcategory, forms.CharField()
* created_date, forms.DateField()

## Schedule
- Week 1
  - Rough landing page, superuser login page and another page for a basic form to send data into post models.

- Week 2
  - Category pages working with subcategories appearing in them. Allow the superuser to edit and delete posts. Possibly fit the search bar functionality into this week.

- Week 3
  - Front-end work, style it up and fix layouts.

- Week 4
  - Stress test the application, fill it with lots of data. If it looks too clunky and unorganized with lots of posts, implement page functions for subcategories.
