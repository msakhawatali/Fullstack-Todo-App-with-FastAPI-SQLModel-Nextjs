<h1 align="center">✅ Fullstack Todo App</h1>

<p align="center">
  Built with <b>FastAPI</b> + <b>SQLModel</b> (Backend) & <b>Next.js</b> (Frontend)  
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9+-blue.svg" />
  <img src="https://img.shields.io/badge/FastAPI-Framework-brightgreen.svg" />
  <img src="https://img.shields.io/badge/SQLModel-Database-orange.svg" />
  <img src="https://img.shields.io/badge/Next.js-Frontend-black.svg" />
  <img src="https://img.shields.io/badge/License-MIT-lightgrey.svg" />
</p>

---

## 🚀 Features

- ✅ User authentication (JWT)  
- ✅ Secure password hashing  
- ✅ CRUD operations for Todos  
- ✅ Each user has their own todos  
- ✅ Input validation & error handling  
- ✅ Modern frontend with Next.js  

---

## 🛠️ Tech Stack

- ⚡ **FastAPI + SQLModel** – Backend & database models  
- 🐘 **PostgreSQL / SQLite** – Database  
- 🔐 **JWT Auth** – Secure login system  
- ⚛️ **Next.js (React)** – Frontend  
- 🚀 **Uvicorn** – ASGI server  

---

## ⚙️ Installation & Setup

### 1. Clone Repository
```bash
git clone https://github.com/msakhawatali/Fullstack-Todo-App-with-FastAPI-SQLModel-Nextjs.git
cd Fullstack-Todo-App-with-FastAPI-SQLModel-Nextjs
````

### 2. Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Create `.env` file in backend:

```env
SECRET_KEY=your_secret_key
ACCESS_TOKEN_EXPIRE_MINUTES=60
DATABASE_URL=sqlite:///./app.db
# or postgresql://user:password@host/dbname
```

Run backend:

```bash
uvicorn main:app --reload
```

➡ `http://127.0.0.1:8000`
➡ Docs: `http://127.0.0.1:8000/docs`

---

### 3. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

➡ `http://localhost:3000`

---

## 📌 API Endpoints (Backend)

| Method | Endpoint       | Description           | Auth |
| ------ | -------------- | --------------------- | ---- |
| POST   | `/auth/signup` | Register a new user   | ❌    |
| POST   | `/auth/login`  | Login & get token     | ❌    |
| GET    | `/users/me`    | Get current user info | ✅    |
| GET    | `/todos/`      | Get all user todos    | ✅    |
| POST   | `/todos/`      | Create a todo         | ✅    |
| GET    | `/todos/{id}`  | Get todo by ID        | ✅    |
| PUT    | `/todos/{id}`  | Update a todo         | ✅    |
| DELETE | `/todos/{id}`  | Delete a todo         | ✅    |

---

## 📂 Project Structure

```
.
├── backend/
│   ├── main.py          # FastAPI entrypoint
│   ├── models.py        # SQLModel models
│   ├── routers/         # API routes
│   ├── schemas/         # Pydantic schemas
│   ├── requirements.txt
│   └── .env
└── frontend/
    ├── pages/           # Next.js pages
    ├── components/      # UI components
    ├── package.json
```

---

## ✅ Running the App

1. Start backend → `uvicorn main:app --reload`
2. Start frontend → `npm run dev`
3. Open browser → `http://localhost:3000`

---

## 🤝 Contributing

1. Fork this repo
2. Create new branch: `git checkout -b feature/xyz`
3. Commit changes & push
4. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License**.

<p align="center">Made with ❤️ using FastAPI + Next.js</p>
