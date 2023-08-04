# Utilities JS
NodeJS project of existing dashboard

## Getting started
To get the Node server running locally:
- Clone this rep
- (optional) Clone the DB to local
- Copy `.env-sample` to `.env` and set the relevant variables
- `npm install` to install all required dependencies
- `npm run build` to initialize all dist files (webpack)
- `npm start` to start the server

## Application Structure
- `.env` - This file contains environment variables and MSSQL credentials
- `bin/www` - The entry point of the application. This files initializes the parameters, requires `app.js` file and defines the express server.
- `app.js` - This file requires the routes and server settings for the application.
- `webpack.config.js` - This file defines the instructions for webpack to build the files for public distribution.
- `src/` - This folder contains the source frontend files to be built by webpack.
- `views/` - This folder contains the base view files.
- `routes/` - This folder contains the route definitions for the application.
- `models/` - This folder contains the models that connects to the database.