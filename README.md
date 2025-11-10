# Full Stack Auth Application

A complete authentication system built with React frontend and Node.js backend.

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

3. Create .env file with:
   ```
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   PORT=5000
   ```

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