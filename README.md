FastAPI User Management API
This is a simple FastAPI application that provides RESTful endpoints for user management with MongoDB as the backend database.

Requirements
Python 3.x
MongoDB
Installation
Clone this repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/fastapi-user-management.git
Navigate to the project directory:

bash
Copy code
cd fastapi-user-management
Install the required Python packages using pip:

bash
Copy code
pip install -r requirements.txt
Running the Application
Make sure MongoDB is installed and running on your local machine.

Start the FastAPI application using uvicorn:

bash
Copy code
uvicorn main:app --reload
The application will be running on http://localhost:8000.

Access the API documentation (Swagger UI) by visiting the following URL in your web browser:

bash
Copy code
http://localhost:8000/docs
Endpoints
POST /users/: Create a new user. Provide the username, password, name, surname, and type (user or admin) in the request body. Returns the newly created user with an autogenerated ID.

GET /users/: Get a list of all users.

GET /users/{user_id}/: Get a specific user by their ID.

GET /users/users/: Get a list of all users with the type "user".

GET /users/admins/: Get a list of all users with the type "admin".

DELETE /users/{user_id}/: Delete a specific user by their ID.

DELETE /users/: Delete all users.

PUT /users/{user_id}/: Update a specific user by their ID. Provide the updated user data in the request body.

POST /login/: User login. Provide the username and password in the request body. If the user exists with the provided credentials, returns the user type.

Usage
You can use tools like curl, Postman, or your web browser to interact with the API endpoints. The API documentation (Swagger UI) provides an interactive interface to test the endpoints directly from the browser.

Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Make sure to adjust the content as per your specific project and requirements. Include additional sections if needed, such as deployment instructions, additional configuration details, or any other relevant information about your application. The README file serves as a helpful guide for users and potential contributors to understand and use your FastAPI application.