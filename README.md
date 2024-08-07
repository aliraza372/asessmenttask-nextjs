# Movies Repository

This repository contains the source code for the Movies application.

## Repository

[https://github.com/faizanhassan-softpers/movies](https://github.com/faizanhassan-softpers/movies)

## Prerequisites

Ensure you have the following installed:

- Node.js
- NPM
- Yarn
- PM2
- Git

## Environment Variables

Create a `.env` file in the root directory of the project and add the following environment variables:

```plaintext
MONGODB_URI=mongodb+srv://movies:movies@movies.8l7wp6i.mongodb.net/movies_db
NEXT_PUBLIC_BASE_URL=http://localhost:3000 
# replace base URL with that of EC2 instance

## Deployment Steps:
- Clone the code
- yarn install
- cp .env.example .env
- Set the above provided env
- yarn build
- sudo pm2 start yarn --name "movies" -- start --port 80
- From browser, go to /api/seed to seed the data.
- Goto base url and login with johndoe@yopmail.com and 12345678 as username and passoword respectively.

