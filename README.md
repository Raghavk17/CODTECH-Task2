**Name:** RAGHAV KUSHWAHA  
**Company:** CODTECH IT SOLUTIONS  
**ID:** CT04DS6323  
**Domain:** Backend  
**Duration:** August to September 2024  
**Mentor:** Muzammil Ahmed  

# Basic Authentication System

## *Overview of the Project*

### *Project*: *Basic Authentication System*

### *Objective*  
The objective of this project is to implement a basic authentication system with registration and login functionality. The system uses Node.js with Express.js for the backend and MongoDB for storing user credentials securely. It includes user registration, login, and token-based authentication.

### *Key Activities*  
- **User Registration**: *Allowing users to create accounts with a username and password.*
- **User Login**: *Authenticating users with stored credentials and generating a token upon successful login.*
- **Data Storage**: *Storing user credentials securely in MongoDB using bcrypt for password hashing.*
- **Token-Based Authentication**: *Using JSON Web Tokens (JWT) to manage user sessions.*

### *Technologies Used*  
- **Node.js**: *JavaScript runtime for server-side development.*
- **Express.js**: *Web framework for building the REST API.*
- **MongoDB**: *NoSQL database for storing user data.*
- **bcrypt**: *Library for hashing passwords securely.*
- **jsonwebtoken**: *Library for creating and verifying JSON Web Tokens (JWT).*
- **HTML/CSS**: *For creating and styling the login and registration pages.*

## *Installation*

1. **Clone the Repository**:
   git clone https://github.com/your-username/your-repository-name.git
   cd your-repository-name

2. **Install Dependencies**:
   npm install
   
3. **Start MongoDB**:
   mongod

4. **Start the Server**:
   npm start

 The server will start on http://localhost:3000.
## *API Endpoints*

- **POST /api/auth/register**
  - **Description**: Registers a new user with a username and password.
  - **Request Body**:
    ```json
    {
      "username": "exampleUser",
      "password": "examplePassword"
    }
    ```
  - **Response**: JSON object with a success message.
  - **Register.html page**
  - ![Screenshot 2024-08-14 162732](https://github.com/user-attachments/assets/89fb11e8-46f2-4896-bbcf-f190f1dc00f5)
  - ![Screenshot 2024-08-14 162756](https://github.com/user-attachments/assets/d5442010-154d-468c-bcd3-c7db80c38116)


- **POST /api/auth/login**
  - **Description**: Authenticates a user and returns a JWT token.
  - **Request Body**:
    ```json
    {
      "username": "exampleUser",
      "password": "examplePassword"
    }
    ```
  - **Response**: JSON object with a token:
    ```json
    {
      "token": "your-jwt-token"
    }
    ```
 - **login.html**
 - ![Screenshot 2024-08-14 162838](https://github.com/user-attachments/assets/a4e227c2-f43f-49b5-b73f-2c771c8f5f6d)
 - ![Screenshot 2024-08-14 162845](https://github.com/user-attachments/assets/0a74b86a-468b-4dd4-8889-2a08006f2616)
- **Mongodb compass output**
- The user information is stored on the mongodb database.
-  ![Screenshot 2024-08-14 162914](https://github.com/user-attachments/assets/c8ef3cbd-6bb7-49de-b349-06e947e30606)

## *Project Structure*

- **public/**
  - **login.html**: HTML file for the login page.
  - **register.html**: HTML file for the registration page.

- **src/**
  - **app.js**: Main server file with routes and server configuration.
  - **authRoutes.js**: Defines authentication-related routes.
  - **userModel.js**: Defines the user schema and model for MongoDB.

- **user-auth/**
  - **node_modules/**: Directory containing project dependencies.
  - **package.json**: Project metadata and dependencies.
  - **package-lock.json**: Dependency versions lock file.
