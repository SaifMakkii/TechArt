# TechArt

<div align="center">
  <h2 style="color: teal;">Welcome to TechArt! 🚀</h2>
  <p><strong>Your cutting-edge blog platform for art, technology, science, cinema, design and food.</strong></p>
</div>

---

## Introduction

**TechArt** is a modern blog platform designed to let users share their passion for art and technology. Built with a **React.js** frontend and an **Express.js** backend, TechArt blends dynamic user interfaces with a robust API service backed by **MySQL**. The platform provides complete user authentication using **JWT** and supports full CRUD operations for posts along with image uploads. Enjoy a beautifully styled layout crafted with **SCSS** for a modern look and responsive experience. 🎨✨

---

## Features

**User Authentication**  
  - Register new accounts and log in securely using hashed passwords and JWT tokens.
**Blog Posts Management**  
  - Create, read, update, and delete posts.
  - Rich text editing powered by **React Quill**.
  - Delete and update options available for posts created by the logged-in user.
**Image Upload and Display**  
  - Upload images associated with each post.
  - Display user profile images and post images dynamically.
**Categorization**  
  - Organize posts by categories such as **Art**, **Science**, **Technology**, **Cinema**, **Design**, and **Food**.
**Responsive Design**  
  - Clean, intuitive UI with responsive elements, leveraging **SCSS** for custom styling.
**API Integration**  
  - Seamless communication between the client and server using **Axios** and **React Router**.
**Security Enhancements**  
  - Cookie parsing and secure access token management for reliable session handling.

---

## Requirements

Before setting up TechArt, please ensure that you have the following tools installed:

| **Tool**         | **Version/Info**                             | **Description**                                      |
|------------------|----------------------------------------------|------------------------------------------------------|
| **Node.js**      | v14 or higher                                | Runtime for running JavaScript on the server         |
| **npm**          | Comes with Node.js                           | Package manager for installing dependencies          |
| **MySQL**        | Latest stable release                        | Database server for blog data storage                |
| **Git**          | Any recent version                           | For cloning and version control                      |

Additionally, the following dependencies are utilized:
**Express.js** – for the backend server.
**React.js** – for the frontend application.
**Axios** – for handling HTTP requests.
**JWT**, **bcryptjs** – for secure authentication.
**React Quill** – for rich text editing.
**SCSS/Sass** – for styling components.

---

## Installation

Follow these steps to set up TechArt on your local machine:

1. **Clone the Repository**  
   Open your terminal and run:
   ```bash
   git clone https://github.com/SaifMakkii/TechArt.git
Install API Dependencies
Navigate to the API directory and install dependencies:
cd TechArt/api
npm install
Install Client Dependencies
Open a new terminal window/tab, navigate to the client directory, then run:
cd TechArt/client
npm install
Database Setup
Ensure MySQL is running.
Create a database named blog (or adjust the configuration in api/db.js as needed).
Usage
To start the project in development mode, follow these instructions:

Start the API Server
In the API folder, run:

npm start
This starts the Express server on port 8800.

Start the Client Application
In the client folder, run:

npm start
This launches the React application. The client proxy is configured to forward API requests to the backend.

Accessing TechArt
Open your browser and visit http://localhost:3000 to see the TechArt homepage. Enjoy browsing, creating, and managing posts!

Configuration
Adjust these configuration files to suit your environment:

Database Connection (api/db.js):
Update the MySQL connection details if necessary.

export const db = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "Saif-183897",
  database: "blog"
});
Backend Routes and Endpoints (api/index.js):

The Express server listens on port 8800.
API endpoints for authentication (/api/auth), posts (/api/posts), and image uploads (/api/upload) are defined.
Client Proxy (client/package.json):
The proxy setting directs API calls to the backend:

"proxy": "http://localhost:8800/api/"
Environment Variables:
Consider moving sensitive information such as database credentials or JWT secret keys to environment variables for better security.

Styling (client/style.scss):
Customize global styling and theme colors by modifying the SCSS files.

Enjoy building and exploring TechArt! 💡🎉
