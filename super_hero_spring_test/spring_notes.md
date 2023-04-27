REST = Representative State Transfer

Stateless requests are sent from a client to either retrieve or makes changes to a resource stored on a server.

In order to provide a response to a request, the server maps the request to an endpoint.

In Spring, a class is marked as a controller and each of its methods is associated with an endpoint.

@RestController annotation is used to declare a class as a controller that can provide application-specific types of data as part of an HTTP response.
    - The @RestController annotation should be added to each class that will handle responses to HTTP request. 
    - It combines functionality of two separate annotations, @Controller and @ResponseBody.

@Controller is used to make a class identifiable to Spring as a component of the web app.

@ResponseBody tells Spring to convert the return values of a controller's methods to JSON and bind that JSON to the HTTP response body.
    - Almost every major programming language offers some type of JSON (JavaScript Object Notation) support.
    - This allows us to easily take an object created in Spring and translate it to JSON which can be easily parsed in the HTML and displayed on the page.

@RequestMapping accepts several arguments. The first and most important is the path.
    - The path argument is used to determine where requests are mapped.
    - For example, if a user makes a request to get a 'book' resource, the server will send the request to a method with the annotation @RequestMapping(path = "/book") and that method would provide the response.

method: allows the developer to specify which HTTP method should be used when accessing the controller method. The most common are:
    - RequestMethod.Get (...Put or ...DELETE)

params: filters requests based on given parameters.

consumes: used to specify which media type can be consumed; some common media types are "text/plain", "application/JSON"