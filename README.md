"Backend Developer Submission - [Abhishek Tiwari]".

## Overview

This repository contains the source code for a ##[real-time chat application] that allows users to communicate efficiently. The application supports multiple clients concurrently and ensures smooth message delivery through robust backend architecture.

### Features

Real-Time Communication: Powered by WebSocket technology.

Secure Backend: Deployed on Render with token-based authentication for secure interactions.

Modern Frontend: Deployed on Vercel with a responsive and interactive interface.

### Access the Deployed Application

Frontend: https://real-time-chat-ten-olive.vercel.app/
Backend: https://real-time-app-j22s.onrender.com
(Backend URL is used internally by the frontend for API and WebSocket communication.)

### Running the Application locally

Prerequisites

Node.js (v16 or higher)
npm (Node Package Manager)
Browser (Chrome, Firefox, or equivalent)

### `Steps to Run the Server`

1.Clone the repository:

git clone https://github.com/Abhicse23/Real-time-chat

2.Install server dependencies:

cd ./server
npm install

3.port=5000
NODE_ENV=production
CORS_ORIGIN=https://real-time-chat-ten-olive.vercel.app/

4.Start the server:
npm start

### `Steps to Run the Frontend`

1.Navigate to the frontend directory:

cd ./client

2.Install dependencies:
npm install

3.Update the ENDPOINT in the client/src/component/Chat/Chat.js/ENDPOINT

const ENDPOINT = 'https://real-time-app-j22s.onrender.com';

4.Start the client application:

npm start


5.Open your browser and visit:
https://real-time-chat-ten-olive.vercel.app/


## Architecture

The application is built using a client-server model:

[Backend (Render):]

Developed in Node.js with Express.js.
Manages API endpoints for user authentication, chat functionality, and WebSocket connections.
MongoDB is used for persistent storage of users and messages.

[Frontend (Vercel):]

Built using React.js.
Communicates with the backend via RESTful APIs and WebSockets.
Optimized for performance and scalability.

[Concurrency Handling:]

WebSockets ensure real-time updates for chat messages.
Asynchronous operations using Promises and event-driven architecture handle concurrent users effectively.


## Assumptions and Design Choices

Hosting Choices:

Render: Chosen for its ease of deployment and auto-scaling for backend services.

Vercel: Ideal for deploying static frontend applications with seamless integration.
Authentication:

Backend endpoints are abstracted through environment variables for flexibility across deployment stages.


## Assumptions and Design Choices

1.Implement typing indicators and read receipts.
2.Add support for media sharing (images, videos).
3.Improve notification mechanisms for offline messages.


## Contact & Support

For any issues, feature requests, or support, please create an issue in this repository or contact:

Name: Abhishek Tiwari
Email: 11abhiofk@gmail.com


















