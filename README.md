Api_practice
============

This is testing repository created from Postman. In this repository placed 3 Postman collections. Detailed descriptions with a list of CRUD operations you can see below.


Practice_2023_https---reqres.in-.postman_collection
---------------------------------------------------

In this collections placed commonnly-used API calls to a free REST API 'https://reqres.in/' with a basik assertions and variables.

* POST Register User
  
  > Registering a user and receiving a token in the response body. Received token and user ID saved into a variable for further using.

 ```JavaScript
// Parse the response body as JSON
var responseBody = pm.response.json();

// Extract the user ID from the response body
var userId = responseBody.id;
var my_token = responseBody.token;

// Save the user ID to an environment variable
pm.environment.set("userId", userId);
pm.environment.set("my_token", my_token);
``` 
  
* POST Create User
* GET Get User List
  
  > Getting a list of users using authorization token, received during registering. 
  
* PUT Update User
* DEL Delete User
* GET Get User By Id


Petstore.postman_collection
---------------------------

In this collection placed commonly-used API calls to a free REST API 'https://petstore.swagger.io/'

* POST Create new pet
* GET Get a pet by id
* PUT Update a pet
* POST Upload an image to existing pet account
  > For correct work download the image from remote repository by link "https://github.com/dziubantaras/Api_practice/blob/main/Iron.jpg?raw=true" and use a local path to a file
* GET Get pets by status
* DEL Delete a pet


API_practice_authorization_GitHub.postman_collection
----------------------------------------------------

In this collection placed a PUT request with an authorization to a 'https://api.github.com'.

* POST Creating a new repository using OAuth 2.0 token.




