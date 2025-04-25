# Chat App Client

## Project Description
This React client application connects to a Node.js backend server using Socket.io to enable real-time chat functionality. It provides a user-friendly interface for sending and receiving messages instantly.

## Why This Technology?
- **React**: For building a responsive and dynamic user interface.
- **Socket.io-client**: Enables real-time, bidirectional communication between client and server.
- **Material UI**: Provides a modern and consistent design system.
- **Emotion**: For flexible and powerful CSS-in-JS styling.

## Basic Setup Steps
1. Ensure Node.js and npm are installed on your machine.
2. Navigate to the `client` directory.
3. Run `npm install` to install all dependencies.
4. Run `npm start` to launch the development server.
5. The app will open automatically in your default browser at `http://localhost:3000`.

## Workflow: How the Technology Works
1. The client establishes a WebSocket connection to the backend server using Socket.io-client.
2. When a user enters a username and joins the chat, the client emits a `join` event to the server.
3. The server registers the user and broadcasts the updated user list and a system message to all clients.
4. When the user sends a message, the client emits a `message` event to the server.
5. The server broadcasts the message to all connected clients with the sender's username and timestamp.
6. The client listens for `message` and `userList` events to update the chat window and user list in real time.
7. When a user disconnects, the server broadcasts the updated user list and a system message.

## Summary
This setup leverages React for UI, Socket.io for real-time communication, and Material UI for styling, creating a seamless and interactive chat experience.

## License
This project is open source and available under the MIT License.
