REST = Representative State Transfer

Stateless requests are sent from a client to either retrieve or makes changes to a resource stored on a server.

In order to provide a response to a request, the server maps the request to an endpoint.

In Spring, a class is marked as a controller and each of its methods is associated with an endpoint.

@RestController annotation is used to declare a class as a controller that can provide application-specific types of data as part of an HTTP response.