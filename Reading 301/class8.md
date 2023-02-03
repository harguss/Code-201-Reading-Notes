# **Reading-Notes**

## Reading 8

## API Design Best Practices

1. What does REST stand for? Representational State Transfer

2. REST APIs are designed around a _REST architectual style -based on a uniform interface.
3. What is an identifier of a resource? Give an example. URI (Uniform Resource Identifier) is a unique sequence of characters that identifies a logical or physical resource used by web technologies. URIs may be used to identify anything, including real-world objects, such as people and places, concepts, or information resources such as web pages and books.
4. What are the most common HTTP verbs?
  GET retrieves resources.
  POST submits new data to the server.
  PUT updates existing data.
  DELETE removes data.
5. What should the URIs be based on?
   It's best when that URI makes sense and adequately describes the resource. URIs should follow a predictable, hierarchical structure to enhance understandability and, therefore, usability.RESTful APIs are written for consumers. The name and structure of URIs should convey meaning to those consumers.
6. Give an example of a good URI.
   <http://api.college.com/students/3248234/courses> - Retrieves a list of all courses that are learned by a student with id 3248234.
   <http://api.college.com/students/3248234/courses/physics> - Retrieves course physics for a student with id 3248234.
7. What does it mean to have a ‘chatty’ web API? Is this a     good or a bad thing?
   Chatty API is one that requires consumer to make tremendous (subjective matter) amount of distinct API calls to get needed information about a resource. A defined chatty API is any API that requires consumer to do more than a single call to perform a single, common operation.
8. What status code does a successful GET request return? 200
  What does 200 OK mean?
   The 200 OK status code means that the request was successful, but the meaning of success depends on the request method used:
   GET: The requested resource has been fetched and transmitted to the message body.
9. What status code does an unsuccessful GET request return?
   An unsuccessful GET request typically returns a 4xx or 5xx HTTP status code. Specifically, a 404 (Not Found) status code indicates that the requested resource could not be found on the server.
10.What status code does a successful POST request return?
   Typically returns a 201(created) HTTP status code, indicating that the resource was successfully created as a result of the request. Another common status code for a succcessful POST request is 200 (ok)which indicates the the request wwas sucessful, but the resource was already present on the server and not modified.
11.What status code does a successful DELETE request return?
   Typically returns a 204(nocontent) HTTP status code, indicating that the requist waw successful  and the server as fulfilled it, but there is no response body to return. Another common status code for a successful DELETE request is 200 (OK), which indicates that the request was successful and the server has fulfilled it, but the response body may include a representation of the deleted resource.

## Bookmark and Review

RegExr -  <https://regexr.com/Pay> particular attention to the cheatsheet
Regex Tutorial  
<https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285>

Regex cookbook — Top 15 Most common regex
<https://medium.com/@fox.jonny/regex-cookbook-most-wanted-regex-aa721558c3c1>

Regex 101 <https://regex101.com/>
