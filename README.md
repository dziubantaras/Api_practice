Api_practice
============

This is test repository created from Postman. In this repository placed 3 Postman collections. Detailed descriptions with a list of CRUD operations you can see below.


Practice_2023_https---reqres.in-.postman_collection
---------------------------------------------------

In this collections placed commononly-used API calls to a free REST API 'https://reqres.in/' with a basik assertions and variables.

* POST Register User
  
> Registering a user and receiving a token in the response body. Received token saved into a variable for further using.

  '''
     const MyData  = pm.response.json();

     pm.environment.set('token', MyData.token)
  
  '''
  
* POST Create User
* GET Get User List
  
> Getting a list of users using authorization token, received during registering. __Token added into Headers section and for some reasons is not visible in saved collection.__
  
* PUT Update User
* DEL Delete User
* GET Get User By Id


Petstore.postman_collection
---------------------------

In this collection placed commononly-used API calls to a free REST API 'https://petstore.swagger.io/'

* POST Create new pet
* GET Get a pet by id
* PUT Update a pet
* POST Upload an image to existing pet account
* GET Get pets by status
* DEL Delete a pet


API_practice_authorization_GitHub.postman_collection
----------------------------------------------------

In this collection placed a PUT request with an authorization to a 'https://api.github.com'.

* POST Creating a new repository using OAuth 2.0 token.




