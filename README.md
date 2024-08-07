Repo:
https://github.com/faizanhassan-softpers/movies
Prerequisites:
Node.js
NPM
Yarn
PM2
Git
.env:
MONGODB_URI=mongodb+srv://movies:movies@movies.8l7wp6i.mongodb.net/movies_db
NEXT_PUBLIC_BASE_URL=http://localhost:3000 
#replace base url with that of ec2
Deployment Steps:
Clone the code
yarn install
cp .env.example .env
Set the above provided env
yarn build
sudo pm2 start yarn --name "movies" -- start --port 80
From browser, go to /api/seed to seed the data.
Goto base url and login with johndoe@yopmail.com and 12345678 as username and passoword respectively.
