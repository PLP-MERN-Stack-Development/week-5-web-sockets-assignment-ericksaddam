[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19925081&assignment_repo_type=AssignmentRepo)
# Real-Time Chat Application with Socket.io

This assignment focuses on building a real-time chat application using Socket.io, implementing bidirectional communication between clients and server.

## Assignment Overview

You will build a chat application with the following features:
1. Real-time messaging using Socket.io
2. User authentication and presence
3. Multiple chat rooms or private messaging
4. Real-time notifications
5. Advanced features like typing indicators and read receipts

## Project Structure

```
socketio-chat/
├── client/                 # React front-end
│   ├── public/             # Static files
│   ├── src/                # React source code
│   │   ├── components/     # UI components
│   │   ├── context/        # React context providers
│   │   ├── hooks/          # Custom React hooks
│   │   ├── pages/          # Page components
│   │   ├── socket/         # Socket.io client setup
│   │   └── App.jsx         # Main application component
│   └── package.json        # Client dependencies
├── server/                 # Node.js back-end
│   ├── config/             # Configuration files
│   ├── controllers/        # Socket event handlers
│   ├── models/             # Data models
│   ├── socket/             # Socket.io server setup
│   ├── utils/              # Utility functions
│   ├── server.js           # Main server file
│   └── package.json        # Server dependencies
└── README.md               # Project documentation
```

## Getting Started

1. Clone the repository:
```bash
git clone https://github.com/PLP-MERN-Stack-Development/week-5-web-sockets-assignment-ericksaddam.git
cd week-5-web-sockets-assignment-ericksaddam
```

2. Install dependencies:
```bash
# Install server dependencies
cd server
npm install

# Install client dependencies
cd ../client
npm install
```

3. Set up environment variables:
   - Create `.env` in the server directory:
     ```
     PORT=5001
     MONGODB_URI=your_mongodb_uri
     JWT_SECRET=your_jwt_secret
     ```
   - Create `.env` in the client directory:
     ```
     VITE_API_URL=http://localhost:5001
     ```

4. Start the application:
```bash
# Start the server (from server directory)
npm run dev

# Start the client (from client directory)
npm run dev
```

## Implemented Features

### Core Features
1. **Real-time Messaging**
   - Instant message delivery
   - Message persistence
   - Optimistic UI updates
   - Message delivery confirmation

2. **User Management**
   - Username-based authentication
   - Online/offline status
   - User presence indicators
   - Profile management

3. **Chat Rooms**
   - Multiple chat room support
   - Room creation and management
   - Room-specific message history
   - Room switching with state preservation

### Advanced Features
1. **Message Enhancements**
   - File attachments
   - Message reactions
   - Read receipts
   - Message search functionality
   - Message pagination

2. **Real-time Interactions**
   - Typing indicators
   - User join/leave notifications
   - Unread message counters
   - Sound notifications
   - Browser notifications

3. **User Experience**
   - Responsive design
   - Loading states
   - Error handling with toasts
   - Reconnection handling
   - Optimistic updates

4. **Performance Optimizations**
   - Message pagination
   - Socket.io room optimization
   - Efficient state management
   - Proper cleanup and memory management

## Technical Implementation

### Client-side Architecture
- React with hooks for state management
- Socket.io-client for real-time communication
- ChakraUI for responsive design
- Custom hooks for socket management
- Error boundary implementation

### Server-side Architecture
- Express.js server
- Socket.io for real-time features
- MongoDB for data persistence
- JWT for authentication
- Room-based message organization

## Screenshots
- Login/Authentication screen
- Main chat interface

## Deployment

[TODO: Add deployment URLs once deployed]
- Frontend: [URL]
- Backend: [URL]

## Resources

- [Socket.io Documentation](https://socket.io/docs/v4/)
- [React Documentation](https://react.dev/)
- [Express.js Documentation](https://expressjs.com/)
- [Building a Chat Application with Socket.io](https://socket.io/get-started/chat)