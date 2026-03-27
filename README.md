# ContractLens — Legal Document Analyzer

Upload any contract (PDF or TXT) and instantly identify risks, obligations, missing clauses, and key dates — explained in plain English.

## Features
- Contract type detection
- Risk identification with severity (high/medium/low) + suggestions
- Plain English summary
- Key dates and obligations extraction
- Missing clause detection
- Chat Q&A about the contract

## Stack
- **Frontend**: React 18, Vite, Tailwind CSS v4, Framer Motion
- **Backend**: FastAPI, Groq SDK, PyPDF2

## Local Development

### Backend
```bash
cd backend && python -m venv venv && source venv/bin/activate
pip install -r requirements.txt && cp .env.example .env
uvicorn main:app --reload --port 8000
```

### Frontend
```bash
cd frontend && npm install
echo "VITE_API_BASE_URL=http://localhost:8000" > .env
npm run dev
```
