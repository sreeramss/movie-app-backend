# Movie App Backend

This is the backend for the movie app project, which uses MongoDB for data storage. It manages user authentication, bookmarks, and data storage, utilizing Express.js and JWT tokens for secure user sessions.

## Features

- **User Authentication:** Handles user login and signup with JWT token creation.
- **Bookmarks Management:** Allows users to add and view bookmarks.
- **Data Storage:** Uses MongoDB to store user and bookmark data.

## Technologies Used

- **Express.js:** Web application framework for Node.js.
- **MongoDB:** NoSQL database for storing user and bookmark data.
- **Mongoose:** MongoDB object modeling for Node.js.
- **JWT:** JSON Web Tokens for secure authentication.

## Installation

1. **Clone the repository:**
    ```sh
    git clone https://github.com/sreeramss/movie-app-backend.git
    cd movie-app-backend
    ```

2. **Install dependencies:**
    ```sh
    npm install
    ```

3. **Create a `.env` file in the root directory and add your environment variables:**
    ```env
    PORT=your_port
    MONGODB_URI=your_mongodb_uri
    JWT_SECRET=your_jwt_secret
    ```

4. **Start the development server:**
    ```sh
    npm start
    ```

5. **API Endpoints:**
    - `POST /signup`: User signup
    - `POST /login`: User login
    - `GET /api/bookmarks`: Get user bookmarks (requires JWT)
    - `POST /api/bookmarks`: Add a bookmark (requires JWT)

## Project Structure

```plaintext
movie-app-backend/
│
├── models/
├── routes/
├── server.js
└── .env
├── .gitignore
├── package.json
└── README.md
