# Poll Fusion

Poll Fusion is a small real-time voting application where users can create polls, share them, and vote instantly. The app uses React on the frontend, Node.js/Express on the backend, Socket.IO for live updates, and MongoDB for storing polls.

Project Live Link - https://poll-fusion.onrender.com

## Features

- Create a poll with 2 to 6 options
- Vote in real time
- See updated results instantly across connected clients
- Browse existing polls
- Responsive React UI

## Tech Stack

- Frontend: React, React Router, Socket.IO Client
- Backend: Express.js, Socket.IO, Mongoose
- Database: MongoDB

## Project Structure

- client/: React frontend
- server/: Express backend and socket server
- server/models/: Mongoose models
- server/routes/: API routes

## Getting Started

### 1. Install dependencies

From the project root, run:

```bash
npm run install-all
```

### 2. Configure environment

Create a `.env` file inside the `server` folder with your MongoDB connection string:

```env
MONGO_URI=mongodb://127.0.0.1:27017/livepoll
```

### 3. Start the app

Run:

```bash
npm start
```

This will start both the client and the server concurrently.

- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## Available Scripts

From the root directory:

- `npm start` — start both frontend and backend
- `npm run server` — start the backend only
- `npm run client` — start the frontend only
- `npm run build` — build the React client
- `npm run start:prod` — build the client and start the backend in production mode
- `npm run install-all` — install dependencies for the root, server, and client

## Notes

- The backend serves the production React build when  app is started in production mode.
- Socket.IO is used for live vote updates inside each poll room.
