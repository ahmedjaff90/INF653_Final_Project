# Ahmed Alzehhawi's INF653_Final_Project
# Deployed Link: https://ahmed-alzehhawi-.glitch.me

Project Overview:
This project involves building a Node.js REST API to manage and interact with data related to US states. The API uses Express for the server framework and MongoDB for data storage, with Mongoose utilized to define the data schema.

Features:
The API is designed to handle a MongoDB collection containing US state data. Each state entry includes its abbreviation, name, and additional fun facts. The API supports a range of CRUD (Create, Read, Update, Delete) operations. For retrieving data, you can use GET requests to fetch all states or data for a specific state by its abbreviation. POST requests allow you to add new states, while PATCH requests enable updating existing state data. DELETE requests are used to remove state data from the collection.

How It Works:
Setup: The project begins with Node.js, and dependencies are managed using npm. Express is used for routing, and Mongoose is employed for database interactions.

Data Modeling: The States.js model defines the schema for state data, including fields such as stateName, stateAbbr, and funFacts. This schema ensures that data is stored consistently in MongoDB.

API Endpoints: The API has several endpoints:

GET /states: Returns a list of all US states.
GET /states/:abbr: Retrieves data for a specific state identified by its abbreviation.
POST /states: Adds a new state to the collection. The request body must include the necessary fields.
PATCH /states/:abbr: Updates data for a specific state. You can include fields to update in the request body.
DELETE /states/:abbr: Deletes data for a state from the collection.
Deployment: The project is deployed on glitch.com, which allows the API to handle requests and interact with the MongoDB database online.

Testing: The API was thoroughly tested to ensure it processes requests correctly. Automated tests were created to validate the functionality of each endpoint.

Usage:
To interact with the API, send HTTP requests to the deployed URL on glitch.com. The API is designed to provide the necessary data or confirmation based on the request made.
