Yelp Clone

A full-stack CRUD web application that replicates the core features of Yelp using the **PERN Stack** — PostgreSQL, Express.js, React.js, and Node.js. Users can browse restaurants, add reviews, and manage data through a responsive frontend backed by a robust API and database.

---

## 🚀 Features

- 🧾 View a list of restaurants with average ratings and reviews
- 📝 Add, edit, and delete restaurants
- 🌟 Submit and delete reviews with real-time updates
- 🌐 RESTful API built with Express and PostgreSQL
- ⚛️ Fully interactive UI with React and Axios

---

## 📦 Tech Stack

| Layer        | Technology       |
|--------------|------------------|
| Frontend     | React, React Router, Axios |
| Backend      | Node.js, Express.js |
| Database     | PostgreSQL |
| Tools        | PG, nodemon, concurrently |

---

## 🛠️ Installation Guide

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/PERN-STACK-YELP-CLONE.git
cd PERN-STACK-YELP-CLONE
2. Set up PostgreSQL
Create a new PostgreSQL database (e.g., yelp)

Run any schema/seed SQL files if provided (in /server/db/)

Example:

sql
Copy
Edit
CREATE DATABASE yelp;
3. Backend Setup
bash
Copy
Edit
cd server
npm install
npm run dev
Make sure to configure your db.js file with your PostgreSQL connection string:

js
Copy
Edit
const { Pool } = require("pg");
const pool = new Pool({
  user: "your_username",
  host: "localhost",
  database: "yelp",
  password: "your_password",
  port: 5432
});
4. Frontend Setup
bash
Copy
Edit
cd ../client
npm install
npm start
The React app will start at http://localhost:3000

📁 Folder Structure
csharp
Copy
Edit
PERN-STACK-YELP-CLONE/
│
├── client/                # React frontend
│   ├── src/
│   └── public/
│
├── server/                # Node + Express backend
│   ├── db/                # PostgreSQL connection and queries
│   └── routes/
│
├── README.md
└── package.json
🔐 Environment Variables (Optional)
Create a .env file in /server/ to store sensitive credentials:

ini
Copy
Edit
DB_USER=your_username
DB_PASSWORD=your_password
DB_HOST=localhost
DB_PORT=5432
DB_NAME=yelp
Make sure to update db.js to use process.env values.

📸 Screenshots
(Add screenshots of the homepage, review page, and forms here)

📌 Known Issues / Todos
Add user authentication (login/signup)

Add filtering by rating/category

Improve UI/UX with animations or transitions

👨‍💻 Author
Prabhat Vaidhya
GitHub Profile — feel free to fork, star, or contribute!
