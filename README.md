# Blog Application 🌐🚀

A simple blog application built with **Express.js**, **MongoDB**, and **EJS** for rendering views. This application supports user authentication for different roles (admin and author), allowing users to create, read, update, and delete blog posts.

## Table of Contents 📃

- [Features](#features)
- [Prereuisites](#prerequisites)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Folder Structure](#folder-structure)
- [User Roles](#user-roles)
- [Usage](#usage)
- [Routes](#routes)
- [User Roles](#user-roles)
- [Contributing](#contributing)
- [License](#license)

## Features 🌟
- **User Authentication**: Sign up and log in with roles (`admin` or `author`).
- **Admin and Author Dashboards**: Separate dashboards for managing posts.
- **File Uploads**: Support for multiple file uploads using **Multer**.
- **Create, Update, and Delete Posts**: Admin and authors can add, edit, or remove posts.
- **Delete Authors**: Admins can delete author accounts.
- **Profile Management**: View posts created by the logged-in user.
- **View Full Post**: Read the full content of a post with all the details.

## Prerequisites ⚙️
Before you begin, ensure you have the following installed on your local machine:
- **Node.js** (version 14.x or later)
- **MongoDB** (Ensure MongoDB server is running on your machine)

## Technologies Used 👨‍💻

- **Node.js**: JavaScript runtime for building server-side applications.
- **Express.js**: Web framework for Node.js.
- **MongoDB**: NoSQL database for storing user and post data.
- **Mongoose**: ODM for MongoDB and Node.js.
- **EJS**: Templating engine for rendering HTML pages.
- **Multer**: Middleware for handling file uploads.
- **Express-Session**: Middleware for managing sessions.

## Installation 🔧

Follow these steps to set up the project locally:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name

2. Install the required dependencies:

   ```bash
   npm install
3. Set up your MongoDB database. Ensure MongoDB is running and create a database named blog.
4. Update the connection string in the code to match your MongoDB setup.

## Folder Structure 📂

| Directory/File        | Description                                   |
|-----------------------|-----------------------------------------------|
| `upload/`             | Directory where uploaded files are stored    |
| `views/`              | Contains EJS templates for rendering pages    |
| `app.js`              | Main server file                             |
| `README.md`           | This README file                             |
| `package.json`        | Project dependencies and scripts             |


## User Roles 🔑

 ### Admin: Can view, add, edit, and delete posts as well as manage author accounts.
 ### Author: Can create posts, update existing posts, and view their own content.

## Usage 💻
1. Start the server

    ```bash
    node index.js

2. Open your browser and navigate to http://localhost:3000 to access the application.


## Routes📡


| Route                | Method | Description                                |
|----------------------|--------|--------------------------------------------|
| `/`                  | GET    | Home page                                  |
| `/login`             | GET    | Login page                                 |
| `/login`             | POST   | Authenticate user                          |
| `/signup`            | GET    | Signup page                                |
| `/signup`            | POST   | Register a new user                        |
| `/logout`            | GET    | Logout user                                |
| `/admin`             | GET    | Admin dashboard (protected)                |
| `/author`            | GET    | Author dashboard (protected)               |
| `/addpost`           | GET    | Add new post page (protected)              |
| `/addpost`           | POST   | Submit new post (protected)                |
| `/updatepost/:title` | GET    | Update post page (protected)               |
| `/updatepost`        | POST   | Submit updated post (protected)            |
| `/deletepost/:title` | GET    | Delete post by title (protected)           |
| `/profile`           | GET    | User profile page (protected)              |
| `/fullpost/:title`   | GET    | View full post by title                    |
| `/deleteauthor`      | GET    | Delete authors page (admin protected)      |
| `/deleteauthor`      | POST   | Delete selected author (admin protected)   |
| `/authordashboard`   | GET    | View authors list (admin protected)        |

## Contributing 🤝
Contributions are welcome! To contribute, follow these steps:

1. Fork the project.
2. Create a new feature branch.
   ```bash
   git checkout -b feature-branch

4. Commit your changes.
   ```bash
   git commit -m "Added a new feature"

6. Push to the branch.
   ```bash
   git push origin feature-branch

8. Open a Pull Request.

## License 📄
This project is licensed under the MIT License. See the LICENSE file for more information.
