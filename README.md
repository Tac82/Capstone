# Kreations

## Overview

* Blog-like application, similar to market websites such as offerup, craigslist, letgo, ect. It will allow one admin user to upload an image, description, price and a search tag to that post.
* The one and only account registered to the application will be an admin. They should be able to edit and delete an item that has already been posted. 
* Clients/customers who visit the applications website should be directed to a homepage with the websites' logo. Interacting with the navbars' search bar or dropdown menu of pre-deteremined tags should direct the client to their requested search or tags. 
* Items that have been posted will be showcased underneath the search tag it is tagged with. 
* Clients who find item(s) they want to order will have to click on the a button in the navbar that directs them to a contact page. This should have the admin's contact information.


## Functionality
Searching for posts/items will be available to unathenticated users, as they can't make an account anyways. However the admin account will need it.
When the admin account wants to make a post, it will instantiate a Posts model with form data.
