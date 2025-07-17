# Nexus App — Legacy Backend

A simple backend for the **Nexus social media app**, built with **Node.js**, **Express**, and **MongoDB Compass** for local development. This backend handles **user registration** and **login**.

---

## 📌 Goals

* Enable users to **sign up** and **log in** to access Home/Profile pages.
* Test credentials:

  * **First name:** Astra
  * **Last name:** Quanta
  * **Email:** [astraquanta@gmail.com](mailto:astraquanta@gmail.com)
  * **Password:** akunnaya1234\$

---

## 🗂️ Project Structure

* `server.js` — main backend entry point; provides REST API endpoints for user registration and login.
* MongoDB Compass used locally for database and collection management.

---

## ⚙️ Local Setup

### 1️⃣ Install dependencies

```bash
npm install --save-dev nodemon
```

Add this script to `package.json`:

```json
"scripts": {
  "start": "nodemon server.js"
}
```

---

### 2️⃣ Set up MongoDB

* Use **MongoDB Compass**.
* Create a database named: **nexus\_db**
* Create a collection named: **users**
* Runs on: `localhost:27017`

---

### 3️⃣ Start the backend server

```bash
npm start
```

* The backend runs `server.js` on **port 5000**.

---

### 4️⃣ Connect frontend to backend

In the **client** (frontend) folder:

```bash
npm install axios
```

* Update `Register.jsx` to make `POST` requests to:
  `http://localhost:5000/register`
* Update `Login.jsx` to make `POST` requests to:
  `http://localhost:5000/login`

---

### 5️⃣ Start the frontend

From the client directory:

```bash
npm run dev
```

* The frontend runs on **port 5173**.

✅ If set up correctly, registration and login requests will hit the backend and store/retrieve user data from MongoDB.

---

## 🌐 Local Ports & Endpoints

| Service            | URL/Port                              |
| ------------------ | ------------------------------------- |
| Frontend (React)   | `http://localhost:5173/`              |
| MongoDB Compass    | `localhost:27017`                     |
| Backend API Server | `http://localhost:5000`               |
| Register Endpoint  | `POST http://localhost:5000/register` |
| Login Endpoint     | `POST http://localhost:5000/login`    |

---

## ✅ Notes

* The **backend** (`server.js`) only provides API endpoints — it does **not** serve any static frontend files.
* All user interactions are handled by the React frontend, which makes HTTP requests to the backend endpoints.

