# CONFIGURATION FOR USER-SERVICE BACKEND

## PRE-REQUISITES
- Make sure to have MongoDB installed and enabled, you can follow
  the installation instructions on the MongoDB official website
  docs here: https://www.mongodb.com/docs/manual/installation/

## SETUP
 - Run `npm install` to install node modules and dependencies

## .env Configuration
- Create a .env file locally at the root of the project directory
- In your .env file, include these variables:
    - MONGO_URI
    - JWT_SECRET
    - REFRESH_TOKEN

### MONGO_URI
Specifies the HOST and PORT your MongoDB database is running on
together with the database to be used in your application. It
usually follow this format: `mongodb://<IP Address>:<PORT>/<DB_NAME>`

### JWT_SECRET
Generate a random token using openssl base64 or any random string
generator to be used for encoding and decoding your web token.
I.e. running this command in your terminal: `openssl base64 32`
should generate a secure random string

### REFRESH_TOKEN
Follow the steps in #JWT_SECRET to generate any random string for
the refresh token.

### STARTUP DEV SERVER
Run `npm run dev` to startup development server

If you see these messages:
```
Server running on port 5000
MongoDB connected
```

It means the backend was properly set up! Congrats!
