# Terminology

Separation of Concerns
    - Which part of the application should be doing this? / Who should be doing this?

# Routing

- Use it to break up an application/api into sub applications
- Picking the code the execute based on URL and HTTP method
- Used for managing sub resources (ex: comments on a blog post)

If you get the errors:
- 'server.listen is not a function', make sure to check that the server is exported properly. Mind the 's' in 'exports' and check that the import = 'require' for the server is correct.
- some errors may also occur if there is another server running on the same port at the same time.
- 'Cannot read property 'use' of undefined = make sure that the variable to the left of the '.' is defined (ex: server.use > make sure server is defined)

# Query String Parameters

- The client can send data to the server inside:
    - the body
    - URL parameters
    - query string parameters (part of the URL)
    - ? headers

(Ex:)
https://www.google.com
/search ------> path (routing handles this)
? ------------> marks the beginning of the query string parameters
source=hp ----> key/value pair
& ------------> separates key/value pairs
