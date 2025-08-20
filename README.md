# 3D To-Do (Django + Next.js)

A beginner-friendly full-stack To-Do app with animated word banner.

## Stack
- Backend: Django + Django REST Framework (SQLite)
- Frontend: Next.js (App Router) + Tailwind + Framer Motion

## Run locally

### Backend
```bash
cd backend
python -m venv .venv
# Windows: .\.venv\Scripts\Activate.ps1
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt  # or: pip install django djangorestframework django-cors-headers
python manage.py migrate
python manage.py runserver 8000

cd ../frontend
cp .env.local.example .env.local  # if you create one
npm install
npm run dev

Open http://localhost:3000

API

GET/POST http://127.0.0.1:8000/api/tasks/

PATCH/DELETE http://127.0.0.1:8000/api/tasks/:id/