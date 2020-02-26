# REST-APIs
Assignment REST APIs

### List of APIs tests:

| Method | URL | Test |
| ------ | ------ |----- |
| GET | [http://httpbin.org/get] | Check that: the request query parameters is completed successfully |
| GET | [http://httpbin.org/get] | Check that: JSON value matches expectation on the request query parameters |
| POST | [http://httpbin.org/post] | Check that: the posting of parameters is completed successfully |
| POST | [http://httpbin.org/post] | Check that: Body matches string on the request post parameters |
| PUT | [http://httpbin.org/put] | Check that: the put parameters is completed successfully |
| PUT | [http://httpbin.org/put] | Check that: Username is correct on the request put parameters |
| DELETE | [https://httpbin.org/delete] | Check that: Checks that deletion is completed successfully |
| DELETE | [https://httpbin.org/delete] | Check that: Checks that deletion time is less than 5 second |
| POST | [http://httpbin.org/response-headers?freeform=Free_1] | Check that: A set of response headers from the query is returning successfully|
| POST | [http://httpbin.org/response-headers?freeform=Free_1] | Check that: Body matches string on a return of a set of response headers from the query string |
| GET | [https://httpbin.org/404] | Check that: Status code is 404, as expected - not found on a not excisting request|
| GET | [https://httpbin.org/404] | Check that: Test error 404 handling: Error message with the error description is in body response |


# RUN TESTS
There are two options of run tests:
#### 1 Using the Postman:

  1. Click the button
  [![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/98d1fe49ba8736de41ce)
  
   *You can download an opensource app (native or or Web View)*
  2. Open App (postman) and sing in
  3. Open collections and find the collection "Assignment Test"
  4. Run the collection
 

#### 2 Using the command line
  1. Download node.js in case you dont have it: 
  https://nodejs.org/es/download/
  2. Install the newman from command line:
    ```
     $ npm install -g newman
    ```
  3. Run the test using the comand: 
    ```
       $ newman run https://www.postman.com/collections/98d1fe49ba8736de41ce
    ```
