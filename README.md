
# 🍞 BakeCart Backend

The backend service for **BakeCart**, a bakery store listing and ordering platform.  
Built with **Node.js**, **Express**, and **MongoDB**.

---

## 🚀 Features
- User authentication (JWT-based)
- Role-based access control (Admin, User)
- Store management API
- Store rating system
- Secure password hashing with bcrypt
- REST API with validation and error handling
- CORS-enabled for frontend integration

---

## 📦 Tech Stack
- **Node.js**
- **Express.js**
- **MongoDB + Mongoose**
- **JWT (JSON Web Tokens)**
- **bcrypt** for password hashing
- **dotenv** for environment variables

---

## 🔧 Installation

1. Navigate to the backend folder:
   ```bash
   cd backend


2. Install dependencies:

   ```bash
   npm install
   ```

3. Start development server:

   ```bash
   npm run dev
   ```

---

## ⚙️ Environment Variables

Create a `.env` file inside `backend/` with:

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/bakecart
JWT_SECRET=your_jwt_secret
CORS_ORIGIN=http://localhost:3000
```

---

## 📂 Project Structure

```
backend/
 ├── config/          # Database config
 ├── controllers/     # Route logic
 ├── middleware/      # Auth & error middleware
 ├── models/          # Mongoose models
 ├── routes/          # Express routes
 ├── utils/           # Helper functions
 ├── server.js        # App entry point
 └── package.json
```

---

## 📜 Scripts

* `npm start` – Start server in production
* `npm run dev` – Start server with nodemon (development)

---

## 🧪 Testing API

Use **Postman** or **cURL** to test API endpoints. Example:

```bash
curl -X POST http://localhost:5000/api/auth/login \
  -H "Content-Type: application/json" \
  -d '{"email": "test@example.com", "password": "12345678"}'
```

---

## 📸 API Endpoints Overview

### Auth

* `POST /api/auth/signup` – Register user
* `POST /api/auth/login` – Login user
* `POST /api/auth/reset-password` – Reset password

### Stores

* `GET /api/stores` – List stores (searchable)
* `GET /api/stores/:id` – Store details
* `POST /api/stores` – Add store (admin only)
* `PUT /api/stores/:id` – Update store (admin only)
* `DELETE /api/stores/:id` – Delete store (admin only)

### Ratings

* `POST /api/stores/:id/rating` – Submit rating
* `GET /api/stores/:id/ratings` – Get store ratings

---

## ✨ Author

Developed by **Gajesh**


