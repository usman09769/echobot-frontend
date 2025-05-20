# Echobot

A simple chatbot interface where the user types a message, and the bot echoes it back. Built with React + TailwindCSS frontend and FastAPI backend.

## Project Structure

```
.
├── backend/
│   ├── main.py
│   └── requirements.txt
└── frontend/
    ├── src/
    │   ├── App.tsx
    │   ├── main.tsx
    │   └── index.css
    ├── index.html
    ├── package.json
    ├── postcss.config.js
    ├── tailwind.config.js
    └── vite.config.ts
```

## Setup Instructions

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the backend server:
   ```bash
   uvicorn main:app --reload
   ```

The backend will be available at http://localhost:8000

### Frontend Setup

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

The frontend will be available at http://localhost:3000

## Features

- Mobile-optimized chat interface
- Real-time message display
- Loading animation while waiting for bot response
- Message bubbles with different colors for user and bot
- Smooth scrolling to latest messages
- Input validation and error handling

## Technologies Used

- Frontend:
  - React
  - TypeScript
  - TailwindCSS
  - Vite
  - Axios

- Backend:
  - FastAPI
  - Python
  - Uvicorn

## API Endpoints

### POST /chat
- Request: `{ "message": "Hello" }`
- Response: `{ "reply": "You said: Hello" }` 