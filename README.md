# Project Backend API

A RESTful Backend API built using **Node.js**, **Express.js**, and **MongoDB**. This project provides authentication, product management, and cart management with JWT-based authorization.

## 🚀 Features

- User Registration
- User Login
- JWT Authentication
- Role-based Authorization (Admin/User)
- Product CRUD Operations
- Cart Management
- MongoDB Database Integration
- Express Middleware
- Error Handling

## 🛠️ Technologies Used

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT (jsonwebtoken)
- bcryptjs
- dotenv
- CORS

## 📁 Project Structure

```
project-backend/
│
├── config/
│   └── db.js
│
├── controllers/
│   ├── authController.js
│   ├── productController.js
│   └── cartController.js
│
├── middleware/
│   ├── authMiddleware.js
│   └── adminMiddleware.js
│
├── models/
│   ├── User.js
│   └── Products.js
│
├── routes/
│   ├── authRoutes.js
│   ├── productRoutes.js
│   ├── cartRoutes.js
│   └── testRoutes.js
│
├── server.js
├── package.json
└── .env
```

## 📦 Installation

Clone the repository:

```bash
git clone <repository-url>
```

Move into the project folder:

```bash
cd project-backend
```

Install dependencies:

```bash
npm install
```

## ⚙️ Environment Variables

Create a `.env` file in the project root.

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

## ▶️ Run the Project

Development Mode

```bash
npm run dev
```

Production Mode

```bash
npm start
```

## 📌 API Endpoints

### Authentication

| Method | Endpoint | Description |
|---------|----------|-------------|
| POST | /api/auth/register | Register User |
| POST | /api/auth/login | Login User |

### Products

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | /api/products | Get All Products |
| GET | /api/products/:id | Get Product By ID |
| POST | /api/products | Create Product |
| PUT | /api/products/:id | Update Product |
| DELETE | /api/products/:id | Delete Product |

### Cart

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | /api/cart | Get Cart |
| POST | /api/cart | Add to Cart |
| DELETE | /api/cart/:id | Remove Item |

## 🔐 Authentication

Protected routes require a JWT token.

Example Header:

```http
Authorization: Bearer YOUR_JWT_TOKEN
```

## 📜 Scripts

```bash
npm start
```

Runs the server.

```bash
npm run dev
```

Runs the server using Nodemon.

This project is for educational and learning purposes.
