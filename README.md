## Backend structure featuring some codes

#### Goals
- Allow users signup and login to view the Home/Profile
- firstname: Astra
- lastname: Quanta
- email: astraquanta@gmail.com
- password: akunnaya1234$

- Allow users modify profile photo, cover photo, age, description and location
- Allow users make post

#### Steps
- Set up Mongodb locally i.e MongoDB Compass. database name: nexus_db. Collection name: users and run in on local host 27017
- local installation: npm install --save-dev nodemon, "scripts": {
  "start": "nodemon server.js"
}
- Server.js
- npm start: starts the backend server.js file (runs on port 5000)

- npm install axios in client folder 
- Modify Register.jsx to make API requests that points to the correct url i.e http://localhost:5000/register
- Modify Login.jsx to make API requests that points to the correct url i.e http://localhost:5000/login
- start the frontend using npm run dev (runs on port 5173)

- Testing successful!

  #### Notes
  - Server.js file provides the API endpoints and does not need to know about the frontend files
  - Frontend files make HTTP requests to these endpoints to handle registration, login, and data fetching
 
  #### Ports and Requests
  - http://localhost:5173/: running in web browswer from VS Code terminal
  - localhost:27017: running in mongodb compass
  - http://localhost:5000: running in VS Code terminal
  - http://localhost:5000/register --> defined in Register.jsx for POST request (frontend file)
  - http://localhost:5000/login --> defined in Login.jsx for POST request (frontend file)
