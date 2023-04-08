# Reading

Status Codes Based On REST Methods

1. In your own words, describe   what each group of status code represents:

100’s = Informational
200’s = Sucess
300’s = Redirection
400’s = Client error
500’s = Server Error

2.What is a status code 202? Accepted
3. What is a status code 308?  Permanent redirect
4. What code would you use if an update didn’t return data to a client? 204 No content
5. What code would you use if a resource used to exist but no longer does? 410 Gone, resouce is no loner availible.
6. What is the ‘Forbidden’ status code? 403 client isnot authorized to acess the requested resource.

## Videos

Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env? So that information is kept private for security against public mischief, and for organization of code.
2. What is middleware? Middleware is used to help integrate different applications that were not originally designed to work together.
3. What does app.use(express.json()) do? When called, app.use(express.json()) enables the server to parse incoming JSON data in a request object.
4. What does the /:id mean in a route? The : character indicates that the following string represents a parameter name. In this case, the parameter is named "id".
5. What is the difference between PUT and PATCH?
6. How do you make a default value in a schema?
7. What does a 500 error status code mean? Server error
8. What is the difference between a status 200 and a status 201?
