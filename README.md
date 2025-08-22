# Melody Search Engine

A web-based melody search engine that helps users identify instrumental music by entering symbolic melodies.

## Project Structure

This is a monorepo containing:
- `apps/api` - Python FastAPI backend
- `apps/web` - React TypeScript frontend
- `packages/shared` - Shared TypeScript types

## Prerequisites

- Node.js >= 18.0.0
- npm >= 9.0.0
- Python >= 3.11

## Setup Instructions

1. **Install dependencies:**
   ```bash
   # Install npm dependencies
   npm install
   
   # Install Python dependencies
   cd apps/api
   pip install -r requirements.txt
   cd ../..
   ```

2. **Build shared types:**
   ```bash
   npm run build:shared
   ```

## Development

Run both frontend and backend development servers:
```bash
npm run dev
```

Or run them separately:
```bash
# Backend only (runs on http://localhost:8000)
npm run dev:api

# Frontend only (runs on http://localhost:5173)
npm run dev:web
```

## Testing

Run all tests:
```bash
npm test
```

Or run tests separately:
```bash
# Backend tests
npm run test:api

# Frontend tests
npm run test:web
```

## API Endpoints

- `GET /api/health` - Health check endpoint
- `GET /` - API root information

## Tech Stack

### Backend
- Python 3.11+
- FastAPI 0.111+
- pytest

### Frontend
- React 18+
- TypeScript 5.4+
- Vite 5+
- Material-UI 5+
- Jest & React Testing Library
