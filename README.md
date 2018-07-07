[![Build Status](https://travis-ci.com/khuynh92/18-oauth.svg?branch=master)](https://travis-ci.com/khuynh92/18-oauth)

Travis: https://travis-ci.com/khuynh92/18-oauth  
Heroku: https://khoa-18-oauth.herokuapp.com  
PR: https://github.com/khuynh92/18-oauth/pull/1  

## 18-oauth


in order to run this app:

 1. clone this repository


 2. in your root folder, create a .env file and set PORT, MONGODB_URI, and APP_SECRET values.  example: 

 ```
 PORT = 3000
 MONGODB_URI = 'mongodb://localhost/lab_18'
 APP_SECRET = 'sssshhhhhhhhh'

 ``` 

 3. First start up your mongo server, and then in your terminal, locate where you cloned this repository, and then type the command: `npm start`. This will begin the server.

 4. in your broswer go to  
`http://localhost:<YOURPORTHERE>`  

 5. Here, you can input fields to test the POST request. The post request will direct you to `http://localhost:<YOURPORTHERE>/post` and show the generated JSON Web Token (jwt) from the post

 6. To test signup(post), use your choice of tools that makes requests to servers (httpie, postman). Without a header that has Basic Authorization, a 401 will be sent. if There is a header object with a Basic Authorizatoin Key, a status code of 200 will be returned with the jwt.

 7. to test the signin(get), ensure that you are signing in using a basic authentication created using the id and password from an existing user




**This lab was built off of codefellows 18-oauth demo code**