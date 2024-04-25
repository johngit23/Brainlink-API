## BrainLink ChatApp API

Welcome to the BrainLink Chat App API! This API is built using Node.js, Express, MongoDB ans SocketIO to power a chat application where users can chat, share files and pictures, create caht groups, and many more. 

## Features

- User Authentication and Authorization: Utilizes JSON Web Tokens (JWT) for secure authentication and authorization to access the API endpoints.
- Commenting System: Users can comment on blog posts and delete their own comments.
- Realtime Communication: employs SocketIO for real time communication.
- Searching Users and accessing their Profile info: Provides endpoints for searching users and checking out their profile.
- Notification of messages: shows notifications of unread messages.
- Profile Management: Users can edit their profile information.

## Technologies Used

- Node.js: A JavaScript runtime built on Chrome's V8 JavaScript engine for server-side development.
- Express.js: A minimalist web framework for Node.js used to build the API endpoints.
- MongoDB: A NoSQL database used for storing blog posts, comments, and user profiles.
- JWT (JSON Web Tokens): Used for user authentication and authorization.
- SocketIO: Used for real-time communication.
- Other Dependencies: Various npm packages such as mongoose for MongoDB object modeling, multer for handling file uploads, etc.

## Installation

- Clone the repository:
  git clone https://github.com/johngit23/Brainlink-API.git
- Navigate to the project directory:
  cd Brainlink-API
- Install dependencies:
  npm install
- Set up environment variables:
  Create a .env file in the root directory and provide the necessary environment variables such as MongoDB connection URI, JWT secret, etc.

- Start the server:
  npm start

## API Endpoints

### Auth

- POST /api/auth/register: Register a new user.
- POST /api/auth/login: Login and obtain JWT token.
- GET /api/auth/logout: Logout a user and remove JWT token.
- GET /api/auth/refetch: Refetch user info when they change.

### Posts

- GET /api/posts: Get all blog posts.
- GET /api/posts/:userId : Get your own posts
- GET /api/posts/:id : Get a specific blog post by ID.
- POST /api/posts/create: Create a new blog post.
- PUT /api/posts/:id: Update an existing blog post.
- DELETE /api/posts/:id: Delete a blog post.

### Users

- GET /api/users: Get all Users.
- POST /api/users: Register User.
- POST /api/users/:id: Login User.

### Comments

- POST /api/comments/create: Comment on a blog post.
- GET /api/comments/:postId: Get comments on a blog post.
- POST /api/comments/:id: Update comment on a blog post.
- DELETE /api/comments/:id: Delete a comment.

## Contributing

Contributions are welcome! Feel free to open issues or pull requests for any improvements or additional features you'd like to see.

## Acknowledgements

Thank you to the developers of Node.js, Express.js, MongoDB, SocketIO and all the npm packages used in this project for making development easier and more efficient. And also to my team mate Margaret Tabby who will be helping me with the frontend for this api.

## Contact
For any inquiries or suggestions, feel free to reach out to jhon.klaus2008@gmail.com.
