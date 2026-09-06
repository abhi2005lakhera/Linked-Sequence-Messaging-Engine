# TalkToMe

TalkToMe is a real-time chat application built with a React frontend and a Node.js/Express backend, using MongoDB for data storage and Socket.IO for real-time messaging.

## Features

- User registration and login
- Real-time one-to-one chat with friends
- Add friends by email
- Unread message notifications
- Last seen/online status
- Persistent chat history

## Project Structure

```
backend/
  controllers/         # Express route controllers (auth, messaging)
  db/                  # Mongoose models and DB connection
  helpers/             # Utility functions (queries, string helpers)
  routes/              # Express route definitions
  index.js             # Main server entry point

frontend/
  public/              # Static assets and HTML template
  src/
    context/           # React context for authentication
    layout/            # Shared layout components (Navbar, MessageBox, etc.)
    App.js             # Main React app
    Home.jsx           # Home page (chat interface)
    Login.jsx          # Login page
    register.jsx       # Registration page
    index.js           # React entry point
```

## Getting Started

### Prerequisites

- Node.js
- MongoDB

### Backend Setup

1. Install dependencies:
   ```sh
   cd backend
   npm install
   ```
2. Create a `.env` file in `backend/` with:
   ```
   URI=<your-mongodb-connection-string>
   ORIGIN=http://localhost:3000
   ```
3. Start the backend server:
   ```sh
   npm run dev
   ```

### Frontend Setup

1. Install dependencies:
   ```sh
   cd frontend
   npm install
   ```
2. Start the frontend:
   ```sh
   npm start
   ```

The frontend will run on [http://localhost:3000](http://localhost:3000) and the backend on [http://localhost:5000](http://localhost:5000).

## Usage

- Register a new account or log in with an existing one.
- Add friends by their email address.
- Start chatting in real time!

## Technologies Used

- React
- Express.js
- MongoDB & Mongoose
- Socket.IO
- Ant Design (UI components)
- Axios

## License

MIT

---

*This is a student project for learning full-stack web development.*