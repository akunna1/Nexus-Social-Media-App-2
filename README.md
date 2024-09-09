## Backend structure featuring some codes

#### Goals
- Allow users signup and login to view the Home/Profile
- firstname: Astra
- lastname: Quanta
- email: astraquanta@gmail.com
- password: akunnaya1234$

#### Steps
- Set up Mongodb locally i.e MongoDB Compass. database name: nexus_db. Collection name: users and run in on local host 27017
- Server.js
- Modify Register.jsx to make API requests that points to the correct url i.e http://localhost:5000/register
- Modify Login.jsx to make API requests that points to the correct url i.e http://localhost:5000/login
- start the backend using node server.js (runs on port 5000)
- start the frontend using npm run dev (runs on port 5173)

  #### Notes
  - Server.js file provides the API endpoints and does not need to know about the frontend files
  - Frontend files make HTTP requests to these endpoints to handle registration, login, and data fetching
