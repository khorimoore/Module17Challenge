Social Network API



Description



The Social Network API is designed to enable a social media application where users can share their thoughts, react to friends’ thoughts, and create a friend list. Built using Express.js for routing, MongoDB for data storage, and Mongoose as the Object Data Modeling (ODM) library, this API serves as the backbone of a social network platform capable of handling large volumes of unstructured data. Additionally, it leverages Moment.js to format timestamps for an enhanced user experience.



Table of Contents



	•	Installation

	•	Usage

	•	Features

	•	Routes

	•	User Routes

	•	Thought Routes

	•	Friend Routes

	•	Reaction Routes

	•	Technologies Used

	•	Contributing

	•	License



Installation



	1.	Clone the repository.



git clone https://github.com/your-username/social-network-api.git





	2.	Navigate to the project directory.



cd social-network-api





	3.	Install dependencies.



npm install





	4.	Set up your MongoDB connection.

	•	Ensure MongoDB is installed and running locally, or use MongoDB Atlas.

	•	Update the MongoDB URI in a .env file if using environment variables for security.

	5.	Start the server.



npm start





	6.	Use Insomnia or Postman to test the routes.



Usage



This API allows developers to create, read, update, and delete (CRUD) operations for users, thoughts, reactions, and friends. The application isn’t deployed; however, Insomnia or Postman can be used for testing each route.



Features



	•	User Management: Add, update, or delete user information.

	•	Thoughts: Users can post their thoughts, which can be edited or deleted.

	•	Friend List: Users can add or remove friends from their friend list.

	•	Reactions: Users can add reactions to thoughts.

	•	Timestamp Formatting: Each thought and reaction includes formatted timestamps for user-friendly date and time.



Routes



User Routes



	•	GET /api/users: Get all users.

	•	GET /api/users/:id: Get a single user by ID.

	•	POST /api/users: Create a new user.

	•	PUT /api/users/:id: Update user details.

	•	DELETE /api/users/:id: Delete a user by ID.



Thought Routes



	•	GET /api/thoughts: Get all thoughts.

	•	GET /api/thoughts/:id: Get a single thought by ID.

	•	POST /api/thoughts: Create a new thought.

	•	PUT /api/thoughts/:id: Update a thought.

	•	DELETE /api/thoughts/:id: Delete a thought.



Friend Routes



	•	POST /api/users/:userId/friends/:friendId: Add a friend to a user’s friend list.

	•	DELETE /api/users/:userId/friends/:friendId: Remove a friend from a user’s friend list.



Reaction Routes



	•	POST /api/thoughts/:thoughtId/reactions: Add a reaction to a thought.

	•	DELETE /api/thoughts/:thoughtId/reactions/:reactionId: Remove a reaction from a thought.



Technologies Used



	•	Express.js: For handling routing and middleware.

	•	MongoDB: NoSQL database for storing users, thoughts, and reactions.

	•	Mongoose: MongoDB ODM library for schema modeling.

	•	Moment.js: For formatting timestamps on thoughts and reactions.

	•	Insomnia/Postman: API testing tools.



Contributing



Contributions are welcome! Feel free to open a pull request to add features, fix bugs, or improve documentation.



License



This project is licensed under the MIT License.



This README gives a complete overview of your API and should help users and developers understand how to install, use, and contribute to the project.