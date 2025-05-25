💬 MERNCOM
A full-featured real-time chat application built using the MERN stack (MongoDB, Express.js, React, Node.js) with Socket.io for real-time communication. This project supports user authentication, instant messaging, and scalable architecture.

This project not only showcases full-stack development but also integrates key Operating System concepts:
 • Concurrency: Node.js handles multiple connections using an event-driven, non-blocking I/O model.
 • Networking: Socket.io enables persistent WebSocket connections for real-time data exchange.
 • Process Management: Nodemon automates server restarts, reflecting OS-level process lifecycle handling.
 • Memory Management: V8 engine and React manage memory efficiently via garbage collection and virtual DOM.
 • Access Control: JWT-based authentication mirrors OS-level permission management.
 • Inter-Process Communication: WebSocket-based communication reflects IPC in distributed systems.

MernCom is both a functional chat platform and a demonstration of how OS principles enhance scalable, real-time web applications.

📁 Project Structure

MERN-Realtime-Chat-Application/
│
├── backend/                  # Express server and API
│   ├── src/
│   │   ├── controllers/      # Request handlers
│   │   ├── middleware/       # Authentication, error handlers
│   │   ├── models/           # Mongoose schemas
│   │   ├── routes/           # API route definitions
│   │   └── lib/              # Utility functions (e.g., DB connection)
│   ├── index.js              # Main server entry
│   ├── package.json
│
├── frontend/                 # React client app
│   ├── src/
│   │   ├── components/       # Reusable UI components
│   │   ├── pages/            # App screens (Login, Chat, etc.)
│   │   ├── context/          # Global state (e.g., Auth, Chat)
│   │   ├── hooks/            # Custom hooks
│   │   └── App.js            # Main React component
│   ├── package.json
│
└── README.md

🚀 Features

🔐 User Authentication (Signup/Login/Logout)
💬 One-to-one Real-time Messaging using Socket.io
🧑‍🤝‍🧑 Online Users Presence Indicator
🔒 Protected Routes (via JWT & Middleware)
📩 Persisted Messages using MongoDB
🧭 Responsive UI (mobile and desktop friendly)
✅ Frontend Form Validation
⚙️ Modular Codebase for scalability

🛠️ Tech Stack & OS Concepts

🔧 Backend
 Node.js – JS runtime using an event loop and non-blocking I/O (Concurrency).
Express.js – REST API framework.

Socket.io –  🔥Real-time communication via WebSockets (Networking).

 • Establishes WebSocket-based bi-directional communication.
 • Falls back to HTTP long-polling if WebSockets aren't supported
 • Enables real-time messaging, typing indicators, and online status
 • Uses event-based architecture: custom events like sendMessage, receiveMessage, userConnected, userDisconnected
 • JWT + Bcrypt – Authentication & password hashing (Access Control & Security)

🎨 Frontend
  React.js – Component-based UI
  Tailwind CSS + Daisy UI – Utility-first responsive styling
  Zustand – Lightweight global state management
  Socket.io-client – Connects browser to server for live communication
    • Listens to and emits events in sync with backend
    • Enables real-time updates without page reloads

🗄️ Database
    MongoDB + Mongoose – NoSQL database with JS-friendly schema

⚙️ Dev Tools
    Nodemon – Auto-restarts server (Process Management)
    Postman – API testing
    VS Code – Development IDE

💡 Key OS Concepts Used
• Concurrency – Async operations in Node.js
• Networking – WebSockets for real-time data transfer
• Process Management – Dev server lifecycle via Nodemon
• Access Control – JWT-based route protection
• Memory Management – Handled by V8 (Node.js engine)

⚙️ Installation & Setup

Prerequisites
• Node.js & npm
 •MongoDB running locally or MongoDB Atlas
• Git

1. Clone the Repository
   • git clone https://github.com/your-username/mern-chat-app.git
   • cd mern-chat-app

2. Backend Setup (/backend)
   • cd backend
   • npm install

• Create a .env file in /backend with the following:
PORT=5001
MONGO_URI=mongodb://localhost:27017/chat_db
JWT_SECRET=your_jwt_secret

• Start the backend server:
npm run dev
Server will run on http://localhost:5001

3. Frontend Setup (/frontend)
   • cd frontend
   • npm install
   • npm start


🧪 API Endpoints
Base URL: http://localhost:5001/api/auth

Method	      Endpoint	          Description
GET          	/signup	            Test Signup route
GET	          /login	            Test Login route
GET	          /logout	            Test Logout route
POST	        /signup            	Register new user
POST	        /login	            Authenticate user


📸 Screenshots



📌 Future Improvements

🗂️ Group chat rooms
📷 Image/file sharing
🔔 Push notifications
🧾 Chat message search
🌍 Deployment to Vercel (frontend) and Render/Heroku (backend)

✨ Acknowledgements

Socket.io Docs
MongoDB Docs
React Official Docs
Zustand





