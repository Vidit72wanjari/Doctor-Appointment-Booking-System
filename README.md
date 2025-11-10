

# 🏥 Full Stack Doctor Appointment System

A complete **doctor appointment booking system** built with **React (Vite)** frontend and **Node.js (Express)** backend, featuring **JWT authentication** and a responsive UI.

---

## 🚀 Features

* User registration and login
* Secure JWT authentication
* Protected routes
* Fully responsive interface
* MongoDB Atlas database (preconfigured)

---

## 📁 Project Structure

```
doctor-appointment-system/
├── backend/
│   ├── package.json
│   ├── server.js
│   ├── .env
│   ├── config/
│   │   └── db.js
│   ├── models/
│   │   └── User.js
│   ├── routes/
│   │   └── authRoutes.js
│   ├── controllers/
│   │   └── authController.js
│   ├── middleware/
│   │   └── authMiddleware.js
│   └── utils/
│       └── generateToken.js
├── frontend/
│   ├── package.json
│   ├── vite.config.js
│   ├── src/
│   │   ├── main.jsx
│   │   ├── App.jsx
│   │   ├── components/
│   │   │   └── ProtectedRoute.jsx
│   │   ├── pages/
│   │   │   ├── Signup.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Home.jsx
│   │   ├── services/
│   │   │   └── api.js
│   │   └── Context/
│   │       └── AuthContext.jsx
│   └── public/
│       └── index.html
└── README.md
```

---

## ⚙️ Setup Instructions

### 🧾 Prerequisites

* Node.js (v14 or higher)
* MongoDB Atlas account (or local MongoDB)
* Git

---

### 🖥️ Backend Setup

1. Navigate to backend folder:

   ```bash
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. This project already includes a **working MongoDB Atlas connection**.
   You **don’t need to change the `.env` file** — just run it.

   ```
   PORT=5000
   MONGO_URI=mongodb+srv://Vidit:Vidit%40123@cluster0.biw23mt.mongodb.net/appointmentDB?retryWrites=true&w=majority
   JWT_SECRET=mysecretkey123
   NODE_ENV=development
   ```

   ✅ Works for everyone since Atlas access is set to `0.0.0.0/0`.

4. Run backend:

   ```bash
   cd backend
   npm install
   npm run dev
   ```

   Backend runs on:
   **[http://localhost:5000](http://localhost:5000)**

---

### 🌐 Frontend Setup

1. Navigate to frontend folder:

   ```bash
   cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create `.env` file:

   ```
   VITE_API_URL=http://localhost:5000/api
   ```

4. Start development server:

   ```bash
   npm run dev
   ```

   Frontend runs on:
   **[http://localhost:3000](http://localhost:3000)**

---

### ⚠️ If it doesn’t connect:

Create your own `.env` file:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=mysecretkey123
NODE_ENV=development
```

Then use your own MongoDB Atlas cluster (free at [https://mongodb.com](https://mongodb.com)).

---

## 🧠 Usage

1. Open your browser → [http://localhost:3000](http://localhost:3000)
2. Sign up with new credentials
3. Log in to view your dashboard
4. Book, view, or manage appointments
5. Log out when done

---

## 🔌 API Endpoints

| Method | Endpoint           | Description         |
| ------ | ------------------ | ------------------- |
| POST   | `/api/auth/signup` | Register a new user |
| POST   | `/api/auth/login`  | Login existing user |

---

## 🛠️ Technologies Used

### Frontend

* React + Vite
* React Router DOM
* Context API
* Axios
* Tailwind CSS / CSS3

### Backend

* Node.js + Express
* MongoDB Atlas + Mongoose
* JWT Authentication
* bcryptjs (password hashing)
* dotenv, cors, nodemon

---

## 🧰 Commands

| Command         | Description                                              |
| --------------- | -------------------------------------------------------- |
| `npm run dev`   | Run both frontend & backend concurrently (if configured) |
| `npm install`   | Install dependencies                                     |
| `npm start`     | Run backend in production mode                           |
| `npm run build` | Build frontend for production                            |

---


---

## 🆘 Support

If you face any issue:

1. Ensure MongoDB is running
2. Check your `.env` variables
3. Verify Node.js version (v14+)
4. Run:

   ```bash
   rm -rf node_modules package-lock.json
   npm install
   ```

---

