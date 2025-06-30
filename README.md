# 📦 WMS API – Warehouse Management System

A simple and secure backend API for managing inventory and orders in a warehouse, built using **Node.js**, **Express**, and **MongoDB**.  
It supports user registration, login, role-based access control, inventory tracking, and order management.

---
## 🚀 Features

- 🔐 JWT-based user authentication
- 🧑‍💼 Role-based access: `admin` and `worker`
- 📦 Inventory management (admin only)
- 📝 Order creation and tracking (all users)
- 📊 MongoDB for persistent data
- ✅ Input validation with Joi
- 🔄 Scalable REST API design

---

## 🔧 Tech Stack

- Node.js
- Express.js
- MongoDB + Mongoose
- Joi (Validation)
- JWT (Authentication)

---

## 🛠️ Setup Instructions

1. **Clone the repo:**
   git clone https://github.com/aryansinha1818/backend_api.git
   cd backend_api
   
2. **Install dependencies:**
   npm install

3. **Create .env file:**
PORT=5000
MONGODB_URI=mongodb://localhost:27017/wms-db
JWT_SECRET=your_jwt_secret
ADMIN_SECRET_KEY=your_admin_secret_key

4. Run the server:
npm start

🔐 Authentication
1. Register with /users/register
2. Provide ADMIN_SECRET_KEY to become admin.
3. Login via /users/login
4. Receive JWT token.

✅ Use token in all protected routes:

✅ Authorization: Bearer <your_token>

📮 API Endpoints Overview
👤 User Routes
POST /users/register – Register user
POST /users/login – Login user

📦 Inventory Routes (Admin Only)
POST /inventory
GET /inventory
GET /inventory/:id
PUT /inventory/:id
DELETE /inventory/:id

📝 Order Routes (All Authenticated Users)
POST /order
GET /order
GET /order/:id
PUT /order/:id
DELETE /order/:id (Admin only)

📬 Postman Collection
Use the provided Postman collection to test the API using different endpoints.
[[Uploading wmp-api.postman_collection.json…]()](https://drive.google.com/file/d/1FQaer7WHkMca_47xCJLCrkm5gWXsRwQA/view?usp=sharing)

Make sure to include your JWT token in the Authorization header for protected routes:
Key: Authorization
Value: Bearer <your_token>

🙋‍♂️ Author
Made with effort and ➡️🎯 & not by ❤️ by Aryan Sinha.

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aryan-sinha-877698212/)

[![gmail](https://img.shields.io/badge/gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:aryan.sinha1818@gmail.com)


   
