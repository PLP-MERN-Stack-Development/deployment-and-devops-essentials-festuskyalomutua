Deployment and DevOps Essentials - MERN Application
Overview

This project demonstrates deployment and DevOps practices for a MERN (MongoDB, Express, React, Node.js) application. It includes best practices for deploying a full-stack app, managing server environments, and ensuring smooth development-to-production workflows.

The backend is a Node.js/Express server, and the frontend is a React client application.

Features

Full-stack MERN application setup

RESTful API with Express and MongoDB

React frontend with modern component structure

Deployment-ready configuration

Environment variable management with .env

DevOps essentials: version control, build scripts, and testing

Project Structure

deployment-and-devops-essentials-festuskyalomutua/

├── client/                 # React frontend

│   ├── public/
│   ├── src/
│   └── package.json

├── server/                 # Node.js backend

│   ├── config/             # Config files (DB connection, environment)
│   ├── controllers/        # Route controllers
│   ├── middleware/         # Custom middleware
│   ├── models/             # Mongoose models
│   ├── routes/             # API routes
│   ├── uploads/            # Uploaded files (if any)
│   ├── package.json
│   └── server.js

├── README.md               # Project documentation

└── WeekX-Assignment.md     # Assignment instructions

Getting Started
Prerequisites

Node.js (v18 or higher)

npm or yarn

MongoDB (local or Atlas)

Git

Installation

Clone the repository:

git clone https://github.com/PLP-MERN-Stack-Development/deployment-and-devops-essentials-festuskyalomutua.git
cd deployment-and-devops-essentials-festuskyalomutua


Install server dependencies:

cd server
npm install


Install client dependencies:

cd ../client
npm install


Set up environment variables:

# Create .env in server/
MONGO_URI=your_mongodb_connection_string
PORT=5000
JWT_SECRET=your_jwt_secret

Running the Application
Server
cd server
npm start

Client
cd client
npm start


Server runs on http://localhost:5000

Client runs on http://localhost:3000

Deployment

The project is structured for deployment on cloud platforms such as Heroku, Render, or Railway.

Build the React client for production:

cd client
npm run build


Serve the build folder with the Express server or a static hosting provider.

DevOps Essentials

Environment variable management for multiple environments (.env, .env.test)

Git version control and branching strategies

Deployment scripts and build automation

Error handling and logging

Testing

Unit, integration, and end-to-end testing can be set up with Jest, Supertest, and Cypress.

Example scripts in package.json:

"scripts": {
  "test": "jest",
  "test:unit": "jest --testPathPattern=tests/unit",
  "test:integration": "jest --testPathPattern=tests/integration",
  "test:e2e": "cypress open"
}

Authors

Festus Kyalo Mutua

GitHub: festuskyalomutua

License

This project is for educational purposes and follows the GitHub Classroom assignment guidelines.
