# Full Stack Doctor Appointment System 

A completeBooking system built with React frontend and Node.js backend.

## Features

- User registration and login
- JWT authentication
- Protected routes
- Responsive UI

## Project Structure

```
fullstack-auth-app/
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

## Setup Instructions

### Prerequisites
- Node.js (v14 or higher)
- MongoDB Atlas account or local MongoDB

### Backend Setup
1. Navigate to backend folder:
   ```
   cd backend
   ```

2. Install dependencies:
   ```
   npm install
   ```



3.This project already includes a working MongoDB Atlas connection.
You don’t need to change the .env file — just run it.

PORT=5000
MONGO_URI=mongodb+srv://Vidit:Vidit%40123@cluster0.biw23mt.mongodb.net/appointmentDB?retryWrites=true&w=majority
JWT_SECRET=mysecretkey123
NODE_ENV=development


 Works for everyone since Atlas access is set to 0.0.0.0/0.

Run backend:

cd backend
npm install
npm run dev


If it doesn’t connect, create your own .env with:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=mysecretkey123
NODE_ENV=development


and use your own MongoDB Atlas cluster (free at mongodb.com
).

4. Start the server:
   ```
   npm start
   ```

### Frontend Setup
1. Navigate to frontend folder:
   ```
   cd frontend
   ```

2. Install dependencies:
   ```
   npm install
   ```

3. Create .env file with:
   ```
   VITE_API_URL=http://localhost:5000/api
   ```

4. Start the development server:
   ```
   npm run dev
   ```

## Usage

1. Open browser and go to `http://localhost:3000`
2. Sign up with your credentials
3. Login to access the home page
4. Logout when done

## API Endpoints

- POST `/api/auth/signup` - User registration
- POST `/api/auth/login` - User login

## Technologies Used

- Frontend: React, Vite, React Router
- Backend: Node.js, Express, MongoDB, JWT
- Authentication: JSON Web Tokens
- Database: MongoDB Atlas
