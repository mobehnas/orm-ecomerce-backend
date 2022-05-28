# orm-ecomerce-backend

## Description
This project was developed using starter code to create a back-end application for an e-commerce site that uses the command line interface (CLI) and object-relational mapping for various methods of data manipulation, storage, and retrieval when using HTTP methods with a RESTUL API.

The schema.sql file in the db folder was run in MySQL Workbench to create the ecommerce_db and establish a connection with Insomnia Core through the command line interface (CLI). Once the database is created, the specific NPM packages are installed using npm i. MySQL2 and Sequelize packages to connect an Express.js API to a MySQL database, which utilizes the dotenv package to store sensitive environmental variables such as: username, password, and database name. npm run seed command migrates the data to MYSQL. A table is created out of the four objects located in the models folder: Product, Category, Tag, ProductTag.

With the node.js packages installed and database seeded without error, run NPM Start to start the server and connect to local host http://localhost:3001/. Then, an API GET request is performed for each route displaying in JSON format. All API POST, PUT, and DELETE routes are tested in Insomnia Core. I am able to successfully create, update, and delete data in my database.

## User Story
  
```
AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies
```
  
## Acceptance Criteria
  
``` 
GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete data in my database
```
  
## Table of Contents
- [Description](#description)
- [User Story](#user-story)
- [Acceptance Criteria](#acceptance-criteria)
- [Table of Contents](#table-of-contents)
- [Installation](#installation)
- [Usage](#usage)

## Installation
 
`npm init`

`npm install mysql2`

`npm install sequelize`

`npm install dotenv`
  
## Usage   
  
Run the following command at the root of your project and answer the prompted questions:

`mysql -u root -p`

Enter PW when promted

`source db/schema.sql`

`quit`

`npm run seed`
  
`npm start`

## Mock-Up

The following animation shows the application’s GET, POST, PUT, and DELETE routes for TAGS being tested in Insomnia Core:

- Create Schema and Seed data: https://drive.google.com/file/d/1zKBLzOfNgHKs7mT24uDTBO1r-Al6G-T1/view
- GET routes to return all categories, all products,all tags : https://drive.google.com/file/d/1_UaePa3MT-A8ox39tBYZztoN_yau0R7s/view
- GET routes to return a single category, a single product,and a single tag : https://drive.google.com/file/d/1lYZtEFkm6T_HtH4PB2AJKwzmYs_WXO1_/view
- POST, PUT, and DELETE routes for categories : https://drive.google.com/file/d/1oRUq-VvjqONG5qxrMYrubyB7imIzySqs/view




