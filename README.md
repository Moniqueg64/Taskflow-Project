
# TaskFlow – Productivity App

**TaskFlow** is a full-stack productivity web app that helps users manage tasks efficiently with a clean UI and secure backend. Built using **React**, **FastAPI**, and **PostgreSQL**, it supports user authentication, task creation, editing, filtering, and deletion.

---

## Features

- User registration and login (JWT-based)
- Create, update, delete tasks
- Set task deadlines and mark as complete/incomplete
- View all tasks in a modern dashboard
- Responsive React frontend
- PostgreSQL database with SQLAlchemy ORM
- Modular backend with FastAPI

---

## Tech Stack

- **Frontend:** React, Vite, Axios, React Router
- **Backend:** FastAPI, SQLAlchemy, JWT, Pydantic
- **Database:** PostgreSQL (Async via asyncpg)
- **Auth:** JWT (Python-Jose, PassLib)
- **Containerization:** Docker-ready (optional)

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/taskflow.git
cd taskflow
```

### 2. Set Up the Backend

Create a `.env` file in `/backend` with:

```env
DATABASE_URL=postgresql+asyncpg://user:password@localhost/taskflow_db
SECRET_KEY=your-secret-key
```

Then install dependencies and run FastAPI:

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### 3. Set Up the Frontend

```bash
cd ../frontend
npm install
npm run dev
```

Frontend runs at `http://localhost:5173`  
Backend runs at `http://localhost:8000`

---

## Folder Structure

```
taskflow/
├── backend/
│   ├── main.py
│   ├── auth/
│   ├── db/
│   ├── models/
│   ├── routes/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
├── requirements.txt
├── package.json
```

---

## Future Features

- Task categories and labels
- Email reminders
- Drag-and-drop task reordering
- Full Docker + Nginx deployment

---

## License

MIT License

---

## Author

Built with purpose by **Monique64**  
GitHub: [@Monique64](https://github.com/Monique64)
