* * *

## What is HTTP?

The Hypertext Transfer Protocol (HTTP) is designed to enable communications between clients and servers.

HTTP works as a request-response protocol between a client and server.

Example: A client (browser) sends an HTTP request to the server; then the server returns a response to the client. The response contains status information about the request and may also contain the requested content.

* * *

## HTTP Methods

*   **GET**
*   **POST**
*   **PUT**
*   **HEAD**
*   **DELETE**
*   **PATCH**
*   **OPTIONS**
*   **CONNECT**
*   **TRACE**

The two most common HTTP methods are: GET and POST.

* * *

## The GET Method

GET is used to request data from a specified resource.

Note that the query string (name/value pairs) is sent in the URL of a GET request:

/test/demo_form.php?name1=value1&name2=value2

**Some notes on GET requests:**

*   GET requests can be cached
*   GET requests remain in the browser history
*   GET requests can be bookmarked
*   GET requests should never be used when dealing with sensitive data
*   GET requests have length restrictions
*   GET requests are only used to request data (not modify)

* * *

## The POST Method

POST is used to send data to a server to create/update a resource.

The data sent to the server with POST is stored in the request body of the HTTP request:

POST /test/demo_form.php HTTP/1.1  
Host: w3schools.com

name1=value1&name2=value2

**Some notes on POST requests:**

*   POST requests are never cached
*   POST requests do not remain in the browser history
*   POST requests cannot be bookmarked
*   POST requests have no restrictions on data length

* * *

## Compare GET vs. POST

The following table compares the two HTTP methods: GET and POST.

<table><tbody><tr><th>&nbsp;</th><th>GET</th><th>POST</th></tr><tr><td>BACK button/Reload</td><td>Harmless</td><td>Data will be re-submitted (the browser should alert the user that the data are about to be re-submitted)</td></tr><tr><td>Bookmarked</td><td>Can be bookmarked</td><td>Cannot be bookmarked</td></tr><tr><td>Cached</td><td>Can be cached</td><td>Not cached</td></tr><tr><td>Encoding type</td><td>application/x-www-form-urlencoded</td><td>application/x-www-form-urlencoded or multipart/form-data. Use multipart encoding for binary data</td></tr><tr><td>History</td><td>Parameters remain in browser history</td><td>Parameters are not saved in browser history</td></tr><tr><td>Restrictions on data length</td><td>Yes, when sending data, the GET method adds the data to the URL; and the length of a URL is limited (maximum URL length is 2048 characters)</td><td>No restrictions</td></tr><tr><td>Restrictions on data type</td><td>Only ASCII characters allowed</td><td>No restrictions. Binary data is also allowed</td></tr><tr><td>Security</td><td>GET is less secure compared to POST because data sent is part of the URL<p>Never use GET when sending passwords or other sensitive information!</p></td><td>POST is a little safer than GET because the parameters are not stored in browser history or in web server logs</td></tr><tr><td>Visibility</td><td>Data is visible to everyone in the URL</td><td>Data is not displayed in the URL</td></tr></tbody></table>

* * *

* * *

## The PUT Method

PUT is used to send data to a server to create/update a resource.

The difference between POST and PUT is that PUT requests are idempotent. That is, calling the same PUT request multiple times will always produce the same result. In contrast, calling a POST request repeatedly have side effects of creating the same resource multiple times.

* * *

## The HEAD Method

HEAD is almost identical to GET, but without the response body.

In other words, if GET /users returns a list of users, then HEAD /users will make the same request but will not return the list of users.

HEAD requests are useful for checking what a GET request will return before actually making a GET request - like before downloading a large file or response body.

* * *

## The DELETE Method

The DELETE method deletes the specified resource.

* * *

## The PATCH Method

The PATCH method is used to apply partial modifications to a resource.

* * *

## The OPTIONS Method

The OPTIONS method describes the communication options for the target resource.

* * *

## The CONNECT Method

The CONNECT method is used to start a two-way communications (a tunnel) with the requested resource.

* * *

## The TRACE Method

The TRACE method is used to perform a message loop-back test that tests the path for the target resource (useful for debugging purposes).