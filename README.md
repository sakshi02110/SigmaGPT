# 🚀 SigmaGPT – AI-Powered Chat Application

![GitHub Repo Size](https://img.shields.io/github/repo-size/sakshi02110/SigmaGPT)
![GitHub Stars](https://img.shields.io/github/stars/sakshi02110/SigmaGPT?style=social)
![Issues](https://img.shields.io/github/issues/sakshi02110/SigmaGPT)
![MIT License](https://img.shields.io/badge/License-MIT-green.svg)
![Built With](https://img.shields.io/badge/Built%20With-React%20%7C%20Node.js%20%7C%20MongoDB-blue)
![OpenAI API](https://img.shields.io/badge/OpenAI-GPT--4o--mini-orange)

---

# 🌟 SigmaGPT

**SigmaGPT** is a full-stack AI-powered chat application that delivers intelligent, conversational experiences using **OpenAI GPT-4o-mini**. It supports multi-threaded chats, message persistence, real-time AI replies, markdown rendering, syntax highlighting, and a sleek ChatGPT-style interface.

This project demonstrates modern full-stack engineering using **React + Vite**, **Node.js + Express**, **MongoDB + Mongoose**, and the **OpenAI API**.

---

# ✨ Features

### 🧠 AI-Powered Chat

* Real-time responses using GPT-4o-mini
* Smooth typing animation
* Markdown + code syntax highlighting

### 🔄 Multi-Threaded Conversations

* Create, switch, and delete chat threads
* Messages stored per thread
* Auto-update titles and timestamps

### 💾 Persistent Storage (MongoDB)

* Stores messages, threads, timestamps
* Fast retrieval via nested message structure

### 🎨 Modern UI (React + Vite)

* Clean ChatGPT-like interface
* Highlighted active thread
* Smooth animations and responsive design

### 🔌 RESTful Backend

* Secure OpenAI integration
* Modular and scalable route structure
* Full CRUD operations for threads & chats

### 🔐 Secure Architecture

* Uses `.env` for API keys & DB URIs
* Backend-only OpenAI calls

---

# 🧩 Tech Stack

### **Frontend**

* React
* Vite
* React Context API
* React Markdown
* Highlight.js

### **Backend**

* Node.js
* Express.js
* Mongoose
* Dotenv

### **Database**

* MongoDB

### **AI Model**

* OpenAI GPT-4o-mini

---

# 📂 Project Structure

```
SigmaGPT
│
├── Backend
│   ├── models
│   ├── routes
│   ├── utils
│   ├── server.js
│   └── .env
│
└── Frontend
    ├── src
    │   ├── components
    │   ├── assets
    │   ├── App.jsx
    │   └── MyContext.jsx
    └── vite.config.js
```

---

# ⚙️ Installation & Setup

## 1️⃣ Clone Repository

```bash
git clone https://github.com/sakshi02110/SigmaGPT.git
cd SigmaGPT
```

---

# 🛠️ Backend Setup

```bash
cd Backend
npm install
```

Create a `.env` file:

```
OPENAI_API_KEY=your_openai_key_here
MONGO_URI=your_mongo_connection_string
PORT=8080
```

Start backend:

```bash
npx nodemon server.js
```

---

# 💻 Frontend Setup

```bash
cd Frontend
npm install
npm run dev
```

Vite will start at:

```
http://localhost:5173
```

---

# 📡 API Endpoints

### **POST /api/chat**

Send a user message and get AI response.

### **GET /api/thread**

Fetch all threads.

### **GET /api/thread/:threadId**

Fetch messages of a specific thread.

### **DELETE /api/thread/:threadId**

Delete selected thread.

---

# 🔥 How It Works

1. User sends a message.
2. Frontend sends `message + threadId` to backend.
3. Backend stores message → calls OpenAI → stores reply.
4. Returns assistant reply.
5. UI updates with animations & markdown formatting.

---

# 🚀 Future Enhancements

* User authentication
* Rename threads
* Voice input
* Model switching
* Cloud deployment

---

# 🤝 Contributing

PRs and suggestions are welcome!

---

# 📜 License

This project is licensed under the **MIT License**.
