# Website API Documentation

This API documentation outlines the routes available for interacting with the website through API requests.# test


## Task API

### Get All Tasks
GET /tasks
- Description: Retrieve all tasks
- Authentication: Required
- Query Parameters:
  - Available query parameters for filtering, pagination, and sorting
- Response:
  - `totalTasks`: Total number of tasks
  - `page`: Current page number
  - `limit`: Number of tasks per page
  - `tasks`: Array of tasks

### Get Task by ID
- Description: Retrieve a task by ID
- Authentication: Required
- Response: Task object

### Create Task
- Description: Create a new task
- Authentication: Required
- Request Body:
  - `description`: Task description
  - `completed`: Task completion status
- Response: Created task object

### Update Task
- Description: Update a task by ID
- Authentication: Required
- Request Body: Updated task fields
- Response: Updated task object

### Delete Task
- Description: Delete a task by ID
- Authentication: Required
- Response: Deleted task object

## User API

### Get Current User
- Description: Retrieve current user profile
- Authentication: Required
- Response: Current user object

### Update User
- Description: Update current user profile
- Authentication: Required
- Request Body: Updated user fields
- Response: Updated user object

### Delete User
- Description: Delete current user profile
- Authentication: Required
- Response: Deleted user object

### Register User
- Description: Register a new user
- Request Body:
  - `username`: User's username
  - `email`: User's email
  - `password`: User's password
- Response: New user object and authentication token

### User Login
- Description: User login
- Request Body:
  - `email`: User's email
  - `password`: User's password
- Response: User object and authentication token

### User Logout
- Description: Log out the current user from all devices
- Authentication: Required
- Response: Success message

### Upload User Avatar
- Description: Upload user avatar
- Authentication: Required
- Form Data: Avatar file
- Response: Base64 encoded avatar

### Get User Avatar
- Description: Get user avatar by user ID
- Response: User avatar image

### Delete User Avatar
- Description: Delete user's avatar
- Authentication: Required
- Response: Success message
