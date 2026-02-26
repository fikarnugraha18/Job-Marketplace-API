🚀 Job Management REST API

A production-ready REST API built with Node.js, Express, PostgreSQL, and Prisma ORM. This project demonstrates backend architecture,authentication, authorization, and clean code structure suitable for real-world applications.

.

📌 About This Project

This backend system simulates a job management platform where:
- Users can register and login securely
- Companies can create and manage job postings
- Admins can manage system-level operations
- Role-based access control is implemented
- Secure authentication using JWT

This project was built to demonstrate production-ready backend development skills.

🛠 Tech Stack

- Node.js
- Express.js
- PostgreSQL
- Prisma ORM
- JWT Authentication
- Bcrypt
- RESTful API Design

✨ Features

- 🔐 User Registration & Login
- 🔑 JWT Authentication
- 🛡 Role-Based Authorization (ADMIN / COMPANY / USER)
- 📄 CRUD Job Management
- 🧠 Clean Architecture (Controller → Service → Prisma)
- ⚠️ Centralized Error Handling
- 🌍 Environment Variable Configuration

📂 Project Structure

```
src/
 ├── applications/     # Business logic layer
 ├── auth/             # Authentication module
 ├── companies/        # Company module
 ├── jobs/             # Job module
 ├── middlewares/      # Auth & error middleware
 ├── config/           # Configuration setup
 ├── lib/              # Utilities & helpers
 ├── modules/          # Feature-based modules
 ├── routes/           # Route definitions
 ├── types/            # Type definitions (TypeScript)
 ├── app.ts            # Express app configuration
 └── server.ts         # Server entry point


 ⚙️ Installation & Setup
1️⃣ Clone Repository
git clone https://github.com/yourusername/yourrepo.git
cd yourrepo

2️⃣ Install Dependencies
npm install

3️⃣ Setup Environment Variables

Create .env file:

DATABASE_URL="your_database_url"
JWT_SECRET="your_secret_key"

4️⃣ Run Migration
npx prisma migrate dev

5️⃣ Start Development Server
npm run dev

Server will run at:

http://localhost:3333

🔑 API Endpoints

Authentication
POST   /auth/register
POST   /auth/login
Jobs
GET    /jobs
GET    /jobs/:id
POST   /jobs        (COMPANY only)
PATCH  /jobs/:id    (COMPANY only)
DELETE /jobs/:id    (ADMIN only)
🧠 What This Project Demonstrates

Secure authentication implementation

Role-based authorization middleware

Proper project structure separation

Production-ready backend setup

Understanding of RESTful principles

📌 Future Improvements

-Pagination & filtering
-Swagger documentation
-Unit testing with Jest
-Docker support
-CI/CD pipeline

👨‍💻 Author

Zulfikar Satya Nugraha
Backend / Fullstack Developer
Indonesia 🇮🇩