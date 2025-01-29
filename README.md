# TodoApp_Backend

This is a simple To-Do List API  where users can create, read, update, and delete tasks in a MongoDB database.

## Features

Add tasks

View all tasks

Edit a task

Delete a task


## Installation and Setup

### 1. Clone the Repository

git clone https://github.com/Jayeshwadlekar/TodoApp_Backend.git

cd todo-app

### 2. Install Dependencies

npm install express mongoose cors dotenv nodemon

### 3. Set Up Environment Variables

Create a .env file in the root directory and add the following:

MONGO_URI=mongodb://localhost:27017/todoDB
PORT=5000

Replace MONGO_URI with your local MongoDB database connection string.

### 4. Start the Server

npm start

### 5. Testing

Use Postman to test the API endpoints.

## API Endpoints

### Method  |  Endpoint  |  Description
**GET**  |   http://localhost:5000/api/tasks    |    Fetch all tasks

**POST**   |  http://localhost:5000/api/task      |   Create a new task

**PUT**   |   http://localhost:5000/api/task/<id>  |  Update a task (Replace <id> with task _id)

**DELETE** |  http://localhost:5000/api/task/<id>  |  Delete a task (Replace <id> with task _id)


### Example JSON Body for POST Request (Create a Task)

> {\
>   "title": "Finish homework",\
>   "description": "Complete the math homework and submit it"\
> }

### Example JSON Body for PUT Request (Update a Task)

> {\
>   "title": "Finish homework",\
>   "description": "Complete math & science homework and submit it",\
>   "completed": true\
> }
