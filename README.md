# Sequelize-Reverse-Engineering-Code

------------------------------------------------------------------------------------------------------------------------------

## PASSWORD AUTHENTICATION

This app allows users to create an account, log into the account and sign back out securely. All user data is stored in a mysql database.

------------------------------------------------------------------------------------------------------------------------------

## USER STORY

As someone who wants to safely log in to "X", I want to know my personal details are safely stored so that I don't have to worry about using "X".

------------------------------------------------------------------------------------------------------------------------------

## TECH USED 

* BCRYPTJS
* EXPRESS
* EXPRESS-SESSION
* MYSQL2
* PASSPORT
* PASSPORT-LOCAL
* SEQUELIZE

------------------------------------------------------------------------------------------------------------------------------

## GETTING STARTED

to begin using this app, please clone this repository into your local storage. Once this is complete, please follow these steps;

1. create a mysql db called "passport_demo"
2. go into the config file, open config.js and insert your personal data ie username, password etc
3. open terminal in current repo and run "npm i" to install all node packages
4. while in terminal, run "node server.js" and you will successfully connect to server
5. open browser and put "http://localhost:8080" in search bar
6. enjoy using the app!

------------------------------------------------------------------------------------------------------------------------------

## FILES EXPLAINED

### CONFIG

  MIDDLEWARE
  
    isAuthenticated.js { 
    restricts routes that a user is not allowed to visit if not logged in. if user is logged in, 
    it continues with request };
    
  config.json {
  connection configuration to connect to server };
  
  passport.js {
  contains javascript logic that tells passport we want to log in with an email address and password };
 
### MODELS

  index.js {
  connects to database and imports users log in data };
  
  user.js {
  requires "bcrypt" for password hashing. This makes our database secure even if compromised. Here we have JS that defines what is stored on our database };
  
### ROUTES

  api-routes.js { 
  contains routes for signing in, logging out and getting users specific data to be displayed client side };
  
  html-routes.js {
  routes that check whether user is signed in, whether user already has account etc and sends them to the correct html page };
  
package.json {
contains all package info, node modules used, version info etc };

server.js {
requires packages, sets up PORT, creates express and middleware, creates routes and syncs database / logs message in terminal on successful connection to server };

------------------------------------------------------------------------------------------------------------------------------
# Model–view–controller

Model–view–controller (usually known as MVC) is a software design pattern commonly used for developing user interfaces that divides the related program logic into three interconnected elements. This is done to separate internal representations of information from the ways information is presented to and accepted from the user.
This kind of pattern is used for designing the layout of the page.

## Components 

### Model

The central component of the pattern. It is the application's dynamic data structure, independent of the user interface. It directly manages the data, logic and rules of the application.

### View 

Any representation of information such as a chart, diagram or table. Multiple views of the same information are possible, such as a bar chart for management and a tabular view for accountants.

### Controller

Accepts input and converts it to commands for the model or view.

## Additional information 

In addition to dividing the application into these components, the model–view–controller design defines the interactions between them.

The model is responsible for managing the data of the application. It receives user input from the controller.
The view means presentation of the model in a particular format.

The controller responds to the user input and performs interactions on the data model objects. The controller receives the input, optionally validates it and then passes the input to the model.

As with other software patterns, MVC expresses the "core of the solution" to a problem while allowing it to be adapted for each system. Particular MVC designs can vary significantly from the traditional description here.[

## The MVC Schema

![mvc-rails](https://user-images.githubusercontent.com/64518932/90301966-9193bc00-ded5-11ea-8ccf-71a0e877038d.png)

# Editable word document 

https://docs.google.com/document/d/1v8qrNm44T2aU5SuHjly3zBXWSl4bkj1KdLB0O14zU3E/edit?usp=sharing