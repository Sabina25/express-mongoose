# Test project

Currently under development.

## Technologies
Simple MVC project using: 
* Express a fast, minimal and flexible web application framework for Node.js
* Mongoose is an Object-Document Mapping (ODM) library for Node.js and MongoDB.
* EJS (Embedded JavaScript) is a templating engine for JavaScript that allows developers to generate dynamic HTML pages

## Installation

To install run the following commands:

````
$ git clone --recursive https://github.com/Sabina25/express-mongoose.git
$ cd express-mongoose
$ npm install
````
To run the application, use the following command:
````
$ npm start 
````

## Introduction
This is a simple project to test your knowledge. The project is a simple MVC application.
Registration is already available, so there is a part of the pages that is available only to the logged in user.
The following pages are currently implemented: 

| PAGE              | LINK                              | Access                             | Functional                                                                                                                                                  |
|-------------------|-----------------------------------|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Singup            | /signup                           | unlogged user                      | New user registration form                                                                                                                                  |
| Login             | /login                            | unlogged user                      | User login form                                                                                                                                             |
| Reset password    | /reset                            | unlogged user                      | Password change form                                                                                                                                        |
| Shop              | /                                 | unlogged user/<br/>logged in user  | List of all products.                                                                                                                                       |
| Products          | /products                         | unlogged user                      | List of available products with the ability to go to a page with detailed <br/> information about a particular product                                      |
| Products          | /products                         | logged in user                     | List of available products with the ability to go to a page with detailed <br/>information about a particular product and add <br/> the product to the card |
| Details           | /products/:productId              | unlogged user/<br/>logged in user  | Page with information about a specific product                                                                                                              |
| Card              | /cart                             | logged in user                     | Information about the current state of the card.<br/> There is also an opportunity to place an order.                                                       |
| Order             | /orders                           | logged in user                     | Information about all orders.                                                                                                                               |
| Add Product       | /admin/add-product                | logged in user                     | Form for adding a new product. Consists of the foll  owing fields:<br/>  1.Title. 2.Price. 3.Image. 4.Description.                                          |
| Pdoducts (Admin ) | /admin/products                   | logged in user                     | List of products with the ability to delete a product or go to the edit page.                                                                               |  
| Edit product      | /admin/edit-product/:productId    | logged in user                     | Editing information about an already existing product.                                                                                                      |  

At the moment, all data is stored on the **MongoDB Atlas cloud service**.
Access to the database is currently only allowed for individual IP addresses.

The **node.bcrypt.js** library is used to encrypt the password.


