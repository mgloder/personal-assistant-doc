# Little Dragon - Personal Assistant Agent

A personal assistant agent that integrates with local software and services, featuring both text and voice chat capabilities.

## Features
- Text-based chat interface
- Voice chat capabilities
- Integration with local software and services
- Modern, responsive UI

## Tech Stack
- Frontend: Next.js with TypeScript
- Backend: Python FastAPI
- AI: OpenAI Agent SDK / MCP
- Voice: Web Speech API

## Setup

### Backend Setup
1. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
```

2. Install dependencies:
```bash
cd backend
pip install -r requirements.txt
```

3. Set up environment variables:
```bash
cp .env.example .env
# Edit .env with your OpenAI API key
```

4. Run the backend:
```bash
uvicorn main:app --reload
```

### Frontend Setup
1. Install dependencies:
```bash
cd frontend
npm install
```

2. Set up environment variables:
```bash
cp .env.example .env.local
# Edit .env.local with your backend URL
```

3. Run the development server:
```bash
npm run dev
```

## Project Structure
```
little_dragon/
├── backend/
│   ├── app/
│   │   ├── agent/
│   │   ├── api/
│   │   └── services/
│   ├── requirements.txt
│   └── main.py
└── frontend/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   └── styles/
    ├── package.json
    └── next.config.js
``` 