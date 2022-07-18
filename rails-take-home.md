# Product Management Tool (Rails/JS)

Your task is to create a simple product management tool that lets you create products and search products in a listing page. You are required to use Ruby on Rails (>=5).

## Requirements

Your app will implement 2 models.
* `Product` which contains the following attributes/validations:
  * `name` (string (0-1024 chars), unique)
  * `upc` (string (10,12 or 13 chars), unique, only numeric characters (0-9) allowed)
  * `available_on` (datetime, must be in the future)
* `Property` which contains the following attributes/validations:
  * `name` (string (0-255 chars), unique)

`Property` will represent additional fields that can be associated with a product. Ex: brand, description, color etc.

Your app will provide 2 pages:

* The Product Create page. This should contain a form with the required Product fields. The form should have a button that lets a user add more properties (name and value pairs) to the product. In the end there should be a save button which lets the user know if validations passed and a record was saved or not. Ex:

![Product Form](https://i.imgur.com/xShO769.png)

* The Listing page. This page lists the products created (in no particular order) and their details (including property name/value pairs). Note that search functionality is optional to search through the products (see "Bonus" section).  Ex:

![Product Listing](https://i.imgur.com/2moVl0h.png)

## Guidelines

* **Your app must be developed using Ruby on Rails (>= 5.0).**
* You may use a database of your choice.
* The Product Create page can be developed using rails templating engine or a front-end framework of your choice (React, Hotwire, etc.). **It's completely up to you to choose.**
* The forms **do not** need to be styled as shown in the example images. You may leave the pages unstyled using only simple html tags if you wish to.
* There is no need to implement any sort of authentication on the app.
* You may use any gem or library in your app to complete your project. Open-source and stackoverflow is your friend.
* Your solution app **must be uploaded to github.com** and **should include a README file** containing instructions on setting up the database and running the app.

## Bonus
* Use React on the FE to implement and render the components
* Add styling with css, either inline or using a styling library of your choice to prettify the pages
* Host your app using Heroku or another service (AWS) so that the finished application can be accessed via a public link.
* Add search functionality on the FE to search through the products on the Listing page.
