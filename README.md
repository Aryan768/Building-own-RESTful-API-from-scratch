# Building-own-RESTful-API-from-scratch
Building own RESTful API from scratch
//jshint esversion:6: This is a comment that sets the version of JavaScript that the code should adhere to (ECMAScript 6).

Import required libraries and modules:

express: Import the Express.js framework, which simplifies building web applications with Node.js.
body-parser: Import the body-parser middleware for parsing incoming HTTP request bodies.
ejs: Import the EJS (Embedded JavaScript) template engine for rendering dynamic web pages.
mongoose: Import Mongoose, a library for working with MongoDB databases.
Create an Express application: Initialize an instance of an Express application.

Configure EJS as the view engine: Set EJS as the template engine for rendering dynamic web pages.

Configure body-parser middleware: Set up body-parser to parse URL-encoded form data.

Serve static files: Use Express to serve static files from a directory named "public."

Connect to MongoDB: Establish a connection to a MongoDB database named "wikiDB" running locally on port 27017.

Define a MongoDB schema: Create a schema for MongoDB documents with two fields - "title" and "content."

Create a MongoDB model: Create a model named "Article" based on the defined schema. This model will be used to interact with the "articles" collection in the database.

Define routes for all articles (/articles):

Handle HTTP GET requests to retrieve all articles in JSON format from the database.
Handle HTTP POST requests to create a new article by adding it to the database.
Handle HTTP DELETE requests to delete all articles from the database.
Define routes for individual articles (/articles/:articleTitle):
Handle HTTP GET requests to retrieve a specific article by its title from the database in JSON format.
Handle HTTP PATCH requests to update a specific article's content in the database.
Handle HTTP PUT requests to update the entire content of a specific article in the database.
Handle HTTP DELETE requests to delete a specific article from the database.
Start the Express server: Start the server on port 3000, and log a message to the console when the server is successfully started.
In summary, this code sets up a basic RESTful API using the Express framework, connects to a MongoDB database, and defines routes for creating, reading, updating, and deleting articles. It also serves static files and uses the EJS template engine for rendering views (although the view-related code is not present in the provided snippet).
