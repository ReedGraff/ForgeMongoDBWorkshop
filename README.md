# MongoDB for MERN Stack Forge Workshop

A full-stack application for recording and managing an organization of people.

## Project information

This project focuses on integrating CRUD database operations using MERN-stack and helps users get accustomed to integrating MongoDB with front-end frameworks. We will be able to create new members, display their content, edit their information, and delete each recording accordingly!

## Steps to run locally

Clone the project

```bash
  git clone https://github.com/doananhtingithub40102/mern-app.git
```

Go to the project directory

```bash
  cd mern-app
```

Create an Atlas URI connection parameter in `server/.env` with your Atlas URI:
```
ATLAS_URI="mongodb+srv://<username>:<password>@cluster0.6cgz2s1.mongodb.net/?retryWrites=true&w=majority"
PORT=5000
```

Create an hostname on server enviroment variable in `client/.env` with your hostname on server:
```
REACT_APP_YOUR_HOSTNAME="http://localhost:5000"
```

Install dependencies

```bash
  cd server
  npm install
```

```bash
  cd client
  npm install
```

Start the server

```bash
  cd server
  node server.js
```
Start the Client

```bash
  cd client
  npm start
```
  

## Features in the project

- The user can **create** the information of a employee, and managing it.

- **Displaying** the information of employees, including the name, position, and level of the employee.

- Includes **Update** and **Delete** actions.

## Learn More

**FrontEnd**

* To learn React, check out the [React documentation](https://reactjs.org/).

* You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

* Get started with [Bootstrap](https://www.w3schools.com/bootstrap5/index.php), the world's most popular framework for building responsive, mobile-first websites.

**BackEnd**

* [Node.js Tutorial](https://www.w3schools.com/nodejs/default.asp)

* [ExpressJS Tutorial](https://www.tutorialspoint.com/expressjs/index.htm)

**Database**

* [MongoDB Tutorial](https://www.w3schools.com/mongodb/)

* Follow the [Get Started with MongoDB Atlas](https://www.mongodb.com/docs/atlas/getting-started/) guide to create an Atlas cluter, connecting to it, and loading your data.

**Fullstack**

* Learn all about the [MERN stack](https://www.mongodb.com/languages/mern-stack-tutorial) in this step-by-step guide on how to use it by developing a simple CRUD application from scratch.

## Live app

<a href="https://employee-manager-tindoan-xu3i.onrender.com/">Live fullstack MERN app</a>
