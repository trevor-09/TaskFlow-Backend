# ⚙️ TaskFlow Backend

This is the **Node.js + Express backend** for TaskFlow — a full-stack task management application.

> 🔗 **Live API**: [https://todobackend-kqc1.onrender.com](https://todobackend-kqc1.onrender.com)

---

## ✨ Features

- 🔐 JWT-based user authentication (signup/login)
- 📝 Create, read, update, and delete tasks
- ✅ Mark tasks as complete or pending
- 🎯 Assign priority levels (low, medium, high)
- 🕓 Automatically store creation timestamps
- 🌍 CORS-enabled API for frontend access

---

## 🧱 Built With

- **Node.js**
- **Express.js**
- **MongoDB Atlas**
- **Mongoose**
- **bcryptjs** (for password hashing)
- **jsonwebtoken** (for token-based auth)
- **dotenv** (for environment config)

---

## 🛠️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/trevor-09/ToDoBackend.git
cd ToDoBackend
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Create Environment File

Create a `.env` file in the root folder and add:

```env
MONGOURL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### 4. Run the Server

```bash
node index.js
```

Server will run at: `http://localhost:8080`

---

## 📌 API Endpoints

| Method | Route                | Description                  |
|--------|----------------------|------------------------------|
| POST   | /register            | Register a new user          |
| POST   | /login               | Log in and receive JWT token |
| GET    | /tasks               | Get all tasks for the user   |
| POST   | /tasks               | Add a new task               |
| DELETE | /tasks/:id           | Delete a task by ID          |
| PATCH  | /tasks/:id/status    | Toggle task status           |
| PATCH  | /tasks/:id/priority  | Update task priority         |

> All `/tasks` routes require an `Authorization: Bearer <token>` header.

---

## 🔗 Frontend Integration

This backend connects to the frontend hosted at:

- 🗂️ **Frontend Repository**: [ToDoFrontend](https://github.com/trevor-09/ToDoFrontend)  
- 🌐 **Live Frontend**: [https://todofrontend-9d0i.onrender.com](https://todofrontend-9d0i.onrender.com)

---

## 👤 Author

**Abhay Raj**  
🎓 B.Tech Computer Science  
🔗 [LinkedIn](https://linkedin.com/in/your-profile)  
📧 [abhayraj@example.com](mailto:abhayraj@example.com)

---

## 🪄 License

This project is open for educational and personal portfolio use.  
Feel free to fork, modify, and build upon it.

---

> Made with ⚙️ Node.js + ❤️ by Abhay Raj
