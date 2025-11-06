

# 💬 ChatApp — Real-time Messaging Platform

Stay connected with your friends, team, or community in real time! **ChatApp** is a full-stack messaging application powered by the **MERN stack** (MongoDB, Express.js, React, Node.js) and **Socket.io**, offering seamless, real-time communication with a clean and responsive UI.

---

## 🚀 Overview

ChatApp lets users connect instantly through secure real-time chats. From instant message delivery to online status indicators, it provides the complete modern chat experience — all wrapped in a sleek, responsive design.

---

## 🌟 Key Features

✨ **Real-time Messaging** — Messages are delivered instantly using Socket.io
🔐 **User Authentication** — Secure login & signup using JWT tokens
🟢 **Online Presence** — Instantly see who’s active or offline
🎨 **Responsive Design** — Looks great on both desktop and mobile (Tailwind + DaisyUI)
👤 **Smart Profiles** — Automatically generated avatars based on username and gender
📜 **Message History** — Chat history is safely stored in MongoDB
🔍 **Search Users** — Quickly find and start conversations with anyone

---

## 🛠️ Tech Stack

### **Frontend**

* ⚛️ React — Dynamic user interface
* 🧭 React Router DOM — Smooth client-side routing
* 🎨 Tailwind CSS + DaisyUI — Modern, elegant design system
* 💡 Zustand — Lightweight state management
* 🔔 React Hot Toast — Sleek notifications
* 💬 Socket.io Client — Real-time messaging
* 🔗 React Icons — Stylish icon set

### **Backend**

* 🟢 Node.js + Express.js — Fast, scalable API backend
* 🍃 MongoDB + Mongoose — Flexible NoSQL database
* ⚡ Socket.io — Real-time, bidirectional event communication
* 🔐 JWT — Token-based authentication
* 🔑 bcryptjs — Password hashing for security
* 🍪 Cookie Parser — Manage cookies safely

---

## ⚙️ Installation & Setup

### 🔧 Prerequisites

Make sure you have:

* Node.js (v14 or above)
* MongoDB (local or Atlas)
* npm or yarn

### 🖥️ Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file and add the following:

```env
PORT=5000
MONGO_DB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
NODE_ENV=development
```

Then start the backend server:

```bash
npm run server
```

### 💻 Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Now your app runs at:

* **Frontend:** [http://localhost:3000](http://localhost:3000)
* **Backend:** [http://localhost:5000](http://localhost:5000)

---

## 🔗 API Endpoints

### 🧍 Authentication

* `POST /api/auth/signup` → Register new user
* `POST /api/auth/login` → Log in existing user
* `POST /api/auth/logout` → Log out

### 👥 Users

* `GET /api/users` → Fetch all users

### 💬 Messages

* `GET /api/messages/:id` → Fetch conversation history
* `POST /api/messages/send/:id` → Send new message

---

## 🔐 Authentication Flow

* JWT tokens stored in **HTTP-only cookies** for security
* Passwords hashed with **bcryptjs**
* Protected routes verified using **middleware**
* Automatic re-authentication for returning users

---

## ⚡ Real-time Functionality

* 🔁 Instant message delivery
* 🟢 Online/offline user tracking
* ⌨️ Typing indicators *(coming soon)*
* ✅ Read receipts *(coming soon)*

---
