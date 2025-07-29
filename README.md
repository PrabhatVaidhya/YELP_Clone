 Re-creating the README.md content again for the PERN Stack Yelp Clone since the previous download failed

yelp_clone_readme = """
# 🍽️ Yelp Clone – PERN Stack Review Platform

**Developed by Prabhat Vaidhya**

A fully functional clone of the popular Yelp platform built using the **PERN stack** (PostgreSQL, Express.js, React.js, Node.js). This web app enables users to browse, review, rate, and manage restaurants—demonstrating full-stack CRUD functionality, RESTful APIs, and PostgreSQL integration.

---

## 🚀 Key Features

- 🔍 **Search & View Restaurants**
- ✍️ **Add, Update, and Delete Reviews**
- 🌟 **Average Ratings with Star Indicators**
- 🧩 **Dynamic Routes for Restaurant Details**
- 📄 **Backend REST API with PostgreSQL**

---

## 🧰 Tech Stack

| Layer      | Technology Used               |
|------------|-------------------------------|
| Frontend   | React.js, Axios, Context API  |
| Backend    | Node.js, Express.js           |
| Database   | PostgreSQL                    |
| Auth       | (Optional) JWT/Bcrypt (future scope) |

---

## 🧱 Project Structure

pern-yelp-clone/
├── client/ # React frontend
│ └── src/
│ ├── components/
│ ├── routes/
│ └── App.js
├── server/ # Express backend
│ ├── db/ # PostgreSQL queries
│ └── index.js # API setup

yaml
Always show details

Copy

---

## ⚙️ Getting Started

### 📦 Prerequisites

- Node.js
- PostgreSQL
- npm or yarn

### 🚀 Clone and Setup

```bash
git clone https://github.com/prabhat-vaidhya/pern-yelp-clone.git
cd pern-yelp-clone
Backend Setup
bash
Always show details

Copy
cd server
npm install
node index.js
Starts backend server at http://localhost:3001

Frontend Setup
bash
Always show details

Copy
cd ../client
npm install
npm start
Starts frontend React app at http://localhost:3000

🛠️ Database Setup (PostgreSQL)
Create a PostgreSQL database named yelp_clone and run the following SQL:

sql
Always show details

Copy
CREATE TABLE restaurants (
  id SERIAL PRIMARY KEY,
  name VARCHAR(50) NOT NULL,
  location VARCHAR(50) NOT NULL,
  price_range INT NOT NULL CHECK (price_range >= 1 AND price_range <= 5)
);

CREATE TABLE reviews (
  id SERIAL PRIMARY KEY,
  restaurant_id INT REFERENCES restaurants(id),
  name VARCHAR(50) NOT NULL,
  review TEXT NOT NULL,
  rating INT NOT NULL CHECK (rating >= 1 AND rating <= 5)
);
Update connection credentials in server/db/index.js accordingly.

📜 Scripts
Location	Script	Description
client	npm start	Run React app
server	node index.js	Start Express API

🎯 Project Objectives
Practice full CRUD operations with PostgreSQL.

Demonstrate PERN stack architecture.

Explore context-based state management in React.

Simulate a real-world restaurant review system.

📄 License
This project is released under the MIT License.
See the LICENSE file for more information.

👨‍💻 Author
Prabhat Vaidhya


This project is a hands-on demonstration of building RESTful applications with the PERN stack — scalable, modular, and production-ready.
