# Ahmed Alzehhawi's INF653_Final_Project
# Deployed Link: https://ahmed-alzehhawi-.glitch.me


Project Overview
This project focuses on building a Node.js REST API to manage and interact with data related to US states. The API is developed using Express for the server framework and MongoDB for data storage, with Mongoose employed to model the data structure.

Features
Data Management: The API handles a collection of US states, where each entry includes the state’s abbreviation, name, and additional fun facts. The data is stored in a MongoDB collection, structured using a Mongoose schema (States.js model).

CRUD Operations: The API supports the full range of CRUD (Create, Read, Update, Delete) operations:

GET: Retrieve information on all states or a specific state by its abbreviation.
POST: Add new states to the collection, along with relevant data.
PATCH: Update existing state data, such as adding or modifying fun facts.
DELETE: Remove a state’s data from the collection.
Data Expansion: The collection was expanded beyond basic state information to include additional details, such as fun facts, making the API more informative and engaging.

How It Works
Setting Up: The project is initialized with Node.js, and dependencies are managed using npm. Key dependencies include Express for routing and Mongoose for interacting with MongoDB.

Data Modeling: The States.js model file defines the schema for state data, specifying fields like stateName, stateAbbr, and funFacts. This schema ensures consistency and integrity of the data stored in MongoDB.

API Endpoints:

GET /states: Returns a list of all US states in the collection.
GET /states/:abbr: Retrieves data for a specific state, identified by its abbreviation.
POST /states: Adds a new state to the collection. The request body should include all required fields.
PATCH /states/:abbr: Updates data for a specific state. The request body can include any fields that need to be updated.
DELETE /states/:abbr: Deletes a state’s data from the collection.
Deployment: The API is deployed on glitch.com, making it accessible for testing and use. The deployment ensures that the API can handle incoming requests and interact with the MongoDB database seamlessly.

Testing: The API was thoroughly tested to ensure it handles various requests correctly and efficiently. Automated tests were created to validate the endpoints and ensure they function as expected.

Usage
To use the API, you can send HTTP requests to the deployed URL on glitch.com. Each endpoint is designed to respond with the appropriate data or confirmation of the action performed, making it straightforward to integrate into other applications or use as a standalone service.
