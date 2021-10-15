# Busymed Backend 

## Question 1 

## A The application must have 2 roles an admin and a customer
## A client approaches you with requirements to build a product reviewing web based solution where customers go and review products. The application requirements are as follows:
## The application must have 2 roles an admin and a customer
## Customer (name required) can register on the application
## Only the admin can create products (name, product type). There are 2 types of products, home and business.
## The home page will display the products and when you click on the product you will see reviews (textReview and rating between 1-5). This where a customer can add a review (only logged in)
## Any role(even unauthenticated visitors) can see products and reviews 
## Reviews (textReview and rating between 1-5) can be deleted by the owner or an admin.
## The client comes and asks you to add a company (name) to the product so that the customers can also review the company separately. Each product belongs to 1 company, a company can have many products.
## Create a scheduled email which gives all comments for the day sent to the admins
## Extra question: Create an api endpoint which returns reviews and company details for a product



## Question 1 a,b,c,d
* User can signup and signin

## Question 1 a
* User can add and view products

## Question 2 b
* User can update or delete his product


## Question  4 

* User can add reviews for a product
* User can update or delete his review



## Question 5 

## API Endpoints
Method | Route | Description
--- | --- | ---
`POST` | `/api/register` | Create a user
`POST` | `/api/login` | Login an already registered user
`GET` | `/api/products` | View all products
`GET` | `/api/products/:id` | View a single product
`POST` | `/api/products/:productId/reviews` | Create a review for a product
`PUT` | `/api/products/:productId/reviews/:reviewId` | Update a product review
`DELETE` | `/api/products/:productId/reviews/:reviewId` | Delete a product review

## Setup


 
 
  ### How to Install the App 
    ```
    $ git clone  git remote add origin https://github.com/SonwabileLanga/Busymed-Back-End.git
    $ cd Busymed-Back-End.git
    $ composer install
    ```
  - Duplicate and save .env.example as .env and fill in environment variables
    ```
    $ php artisan migrate
    ```
  ### Run The Script
  ```
  $ php artisan serve
  ```


## Technology I use
  - [PHP](https://www.php.net)
  - [Composer](https://getcomposer.org)
  - [MySql](https://www.mysql.com)
  - [Laravel](https://laravel.com)
  git init