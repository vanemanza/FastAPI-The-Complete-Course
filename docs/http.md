
### FastAPI uses HTTP request methods

Fast API excels at quickly  creting  restful APIs, rest APIs uses  same request methods as http.
It tells a server what the request wants to do that is coming in.

Rest APIs typically include:
* GET, read method that retrives data.
* POST, create method, to submit data.
* PUT, update the entire resource.
* PATCH, update part of the resource.
* DELETE, delete the  resource

These operations are also known as the **CRUD** operations, which stands  for create, read, update and delete.

There are some additional request methods:
* TRACE, performs a message loop-back to the  target.
* OPTIONS, describes communication  options to the target.
* CONNECT, creates a tunnel to the server, based on the target resource.

### FastAPI response status code

**1xx** -> **Informational response: request processing**. This is how a client knows if the exchange between the client and the server were successful. When in the 100 level of status code, that means you received an  informational response, which usually means the  server is still processing the request. This is not a failure between the exchange.

**2xx** -> **Success: Request  successfully  complete**. It means the exchange between  the  client and the server were successful.

**3xx** -> **Redirection: Further action must be complete**. 

