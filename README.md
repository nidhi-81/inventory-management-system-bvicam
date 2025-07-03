# Inventory Management System – BVICAM

A full-stack web app for managing inventory and return requests within an educational institute.
Developed as a practical implementation of real-world role-based access, secure authentication, and CRUD operations.

## Roles & Functionalities
### Faculty
- Register and login securely (JWT-based)
- Request items from inventory
- Track request status (Approved/Rejected/Pending)
- Return items (with quantity control)
- View remarks from admin

### Admin
- Add new inventory items and categories
- View, update, and process user requests
- Track return requests and acknowledge them
- Inventory quantity auto-adjusts on request/return

### Super Admin
- Oversee all requests and returns
- Approve/reject requests with remarks
- Full read/write access across system

## Tech Stack
- Frontend :  ReactJS
- Backend : Node.js, Express
- Databse : MSSQL 
- JWT for authentication

## 🛠️ Project Structure

## 🛠️ Project Structure

/stock_mgm
├── /frontend
│ ├── /src
│ │ ├── App.js
│ │ ├── login.js
│ │ ├── signup.js
│ │ ├── facultyDashboard.js
│ │ ├── adminDashboard.js
│ │ ├── superAdminDashboard.js
│ │ └── ...
│ └── .gitignore
├── /backend
│ ├── routes/
│ ├── middleware/
│ ├── db.js
│ ├── .env.example
│ ├── .gitignore
│ └── server.js
├── README.md


### Backend Setup
```bash
cd backend
npm install
cp .env.example .env
# Add your DB credentials and JWT_SECRET in .env
node server.js
```
## Frontend Setup
```bash
cd frontend
npm install
npm start
