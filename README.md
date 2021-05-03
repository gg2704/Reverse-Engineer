# Reverse-Engineer

# The Server.js
The server.js file is your entry point into this Node application. It sits in the root of the project folder and contains the JavaScript coded needed for the Express server to work, serve files and make the page routing work.

# The Routes/
The routes folder contains 2 javascript based source files. One for HTML (the page routes) and one for the API (the API routes) routes. Each file uses an annonymous function (passing in 1 parameter ) upon export so that when we require them in the server.js file we can pass the app constant that we made using express().

As expected, the api-routes files contain the routes for the api and the expected and accepted logic for each HTTP protocol as needed. The same can be said for the html-routes.js file.

# The Public/
The public folder contains all of the files necessary for the front end. This includes all the client side JavaScript, CSS and HTML needed to display the site. The members.html page in this case, acts as the index page when a user is logged in vs when the signup.html page being the default index page when a user is logged out.

We can be sure of this because of the code in the routes/html-routes.js file that references a HTTP GET Request and where to send response.

This code reroutes and index or root route to the /members endpoint if they are logged in, and displays the signup.html page if they are not logged in.
