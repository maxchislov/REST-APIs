# REST-APIs
Assignment REST APIs

### List of APIs tests:

| Method | URL | Test |
| ------ | ------ |----- |
| GET | [http://httpbin.org/get][PlDb] | Check that: Status code is 200 (OK) |
| GET | [http://httpbin.org/get][PlDb] | Check that: JSON value is match expectation |

| POST | [http://httpbin.org/post][PlDb] | Check that: Status code is 200 (OK) |
| POST | [http://httpbin.org/post][PlDb] | Check that: Body matches string |

| PUT | [http://httpbin.org/put][PlDb] | Check that: Status code is 200 (OK) |
| PUT | [hhttp://httpbin.org/put][PlDb] | Check that: Username is correct |

| DELETE | [https://httpbin.org/delete][PlDb] | Check that: Status code is 200 (OK) |
| DELETE | [https://httpbin.org/delete][PlDb] | Check that: Response time is less than 5 second |

| POST | [http://httpbin.org/response-headers?freeform=Free_1][PlDb] | Check that: Status code is 200 (OK) |
| POST | [http://httpbin.org/response-headers?freeform=Free_1][PlDb] | Check that: Body matches string |

| GET | [https://httpbin.org/404][PlDb] | Check that: Status code is 404, as expected - not found |
| GET | [https://httpbin.org/404][PlDb] | Check that: Test error 404 handling: Error message with the error description is in body response |


# RUN TESTS
There is a two options of run tests:
#### 1 Using the Postman:

[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/98d1fe49ba8736de41ce)

You can download an opensource app (native or or Web View)

  1. Open App (postman) and sing in
  2. Find the collection "Assignment Test"
  3. Run the collection
 

#### 2 Using the command line
  1. Download node.js in case you dont have it: 
  https://nodejs.org/es/download/
  2. Install the newman from command line:
  ```sh
     $ npm install -g newman
  ```
  3. Run the test using the comand: 
    ```sh
     $ newman run https://www.postman.com/collections/98d1fe49ba8736de41ce
    ```
