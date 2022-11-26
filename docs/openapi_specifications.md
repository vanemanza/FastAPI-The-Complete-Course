## OAS: OPENAPI SPECIFICATIONS

    The OpenAPI specification, also know as the OAS, is a complete documentation on creating a  universal standard on how to create and handle APIs.
    The way Open API describes a standar is by using languages agnostic interfaces wich allos humans and machines to be able to easily understand what a specific service is doing without understanding the code or having to read the  documentation.
    This overall allows a user to be able to consume and interact with an API with minimal effort.

### OpenAPI Document Defines:

    * Schema: The schema is a abstract definition of what the API should look like. Think of it as a blueprint of how data in the API should look when being created. 
    * Data Format: The data format in which a JSON or Ymal data format should be handled.
    * Data Type: the data types in wich primitive data types are handled througout the  requests and the  responses.
    * Path: is how to handle parameters if the specific API takes any.
    * Object: is how objects should be handled within an API.
  
Open API specifications allows you to be able to write clean code when dealing  with APIs and web services.

### View OpenAPI Schema

* FastAPI generates the open API schema for you to view.

{
    "openapi": "3.0.2",
    "info": {
        "title": "FastAPI",
        "version": "0.1.0"
    },
    "paths": {
        "/": {
            "get": {
                "summary": "First API",
                "operationId": "first_api__get",
                "responses": {
                    "200": {
                        "description": "Successful Response",
                        "content": {
                            "application/json": {
                                "schema": {}
                            }
                        }
                    }
                }
            }
        }
    }
    
...    
}

Within the paths, we only have one API, which can be seen as an empty string and they get request method.

The summary is "First API", which renamed the function, this with  an "operation id" of first API and attach at the end is the request method, which is get. 

The status code  within the response is 200, with a description attached  as a successful response.

* URL: within our application, we can view the entire open API standard by going to your project's URL, followed by Open API json

http://127.0.0.1:8000/openapi.json

Helps developers create restful APIs based on specific clean code and clean API standards, so individuals can  use the APIs easily.






