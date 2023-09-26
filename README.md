# MongoDB for MERN Stack Forge Workshop

A full-stack application for recording and managing an organization of people.

## Project information

This project focuses on integrating CRUD database operations using MERN-stack and helps users get accustomed to integrating MongoDB with front-end frameworks. We will be able to create new members, display their content, edit their information, and delete each recording accordingly!

## How to get started

Clone the project in a directory

```bash
  git clone https://github.com/abhinavkolli03/ForgeMongoDBWorkshop.git
```

Install the appropriate dependencies in EACH the server and client

```bash
  cd server
  npm install
```

```bash
  cd client
  npm install
```

## What about MongoDB Atlas?

Now, we need to walk through making your MongoDB Atlas account, and creating a cluster!

First, make a MongoDB account at the following account if you don't have one... [MongoDB Website](https://www.mongodb.com/)

Now, let's create a cluster and name it unique like ConvergentMongo. We are picking the M0 FREE tier. Once this is set, click create! 

You will need to create a username and password to give yourself full access to the cluster. Lastly, we have the IP Access List. It is good practice to give private access to the cluster as much as possible, but for learning purposes we will largen the CIDR range to access from anywhere with 0.0.0.0/0.

Once the cluster is active, let's connect to it by going to Database and clicking the "MongoDB for VS Code" button under Connect. This will allow us to work directly with our database from our VS Code interface. Let's follow the steps it mentions to setup VS Code with MongoDB. Once you finish this, SAVE YOUR CONNECTION STRING!

# How do we establish this connection?

Before doing anything, we need to provide the private credentials for our database to our client and server files. We can do this using a .env file.

For the `server/.env`, let's add the following variable `ATLAS_URI` and set it to our connection string for our cluster. Change the username and password as necesary. Let's also define the port for the server to run from by saying `PORT=5000`

Then, for the `client/.env`, simply paste the following variable and credentials: 
```
REACT_APP_YOUR_HOSTNAME="http://localhost:5000"
```

This will ensure the react app connects to the appropriate host run on a unique localhost 5000

# How do I run this locally?

Simple!

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

If we have time, we will delve into the code. If not, I highly advise everyone to please go over the code and learn how packages like MongoClient or mongoose communicate with express, CORS, and the app in general.

## Features in the project

- The user can **create** the information of a member, and managing it.

- **Displaying** the information of members, including the name, position, and current occupation status.

- Includes **Update** and **Delete** actions.

## Finale

Hopefully, this helped clarify a few things...
- Establish and create a database with MongoDB
- Connect your cluster with your frontend in VS Code locally
- Understand CRUD operations and their importance
- Analyze metrics and charts provided by MongoDB interface