# Recipe-Management-App

This project provides the backend API for a Recipe Management Application.
It enables users to authenticate, create, view, update, and delete recipes.
The API uses Node.js, Express.js, JWT for authentication, and MongoDB as the database.

## Features

- User Authentication: JWT-based authentication for user registration and login.
- CRUD Operations for Recipes:
- Create, Read, Update, and Delete recipes.
- MongoDB Database: Recipes and user data stored with proper schema design.
- Error Handling :- Proper error handling for this Recipe management App

## Technologies Used

- Node.js
- Express
- MongoDB
- Mongoose
- Bcrypt.js
- body-parser
- cors
- dotenv
- nodemon
- jsonwebtoken
- cookie-parser

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Sujanbutani/Recipe-Management-p-5.git

2. Install dependencies:

    ```bash
    npm install

3. .env file

     ```
    MONGO_URI=your_mongo_db_connection_string
    PORT = "5000"
    JWT_SECRET= "secret key"
    ```

4. Start the development server:

   ```bash
    npm start
    The server should now be running at http://localhost:5000
   ```

## API Endpoints

### User Api
1. User Api (Register-Post) :- localhost:5000/user/signup
2. User Api (login - Post) :- localhost:5000/user/login

### Recipe Api
1. Recipe Api (Post) :- localhost:5000/Recipe/create
    - Requires JWT token in the Authorization header.
2. Recipe Api (Get - Allpost) :- localhost:5000/Recipe/AllRecipe
3. Recipe Api (Get - Onepost) :-  localhost:5000/Recipe/SingleRecipe/<Recipe_id>
4. Recipe Api (Update) :- localhost:5000/Recipe/UpdateRecipe/<Recipe_id>
5. Recipe Api (Delete) :- localhost:5000/Recipe/DeleteRecipe/<Recipe_id>

## Error Handling :-
- 400: Invalid or malformed request.
- 401: Unauthorized access (missing or invalid JWT token).
- 404: Resource not found (e.g., recipe or user).
- 500: Internal server error.

## Environment Variables
- PORT: The port for the server to listen on.
- MONGODB_URI: Your MongoDB connection string.
- JWT_SECRET: Secret key for signing JWT tokens.
