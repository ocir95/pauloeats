# PauloEats - Project Structure

## Overview

PauloEats is structured as a monorepo with separate frontend and backend directories.

## Directory Layout

```
pauloeats/
├── frontend/
│   ├── src/
│   │   ├── components/      # React components
│   │   ├── pages/           # Page components
│   │   ├── services/        # API services
│   │   ├── hooks/           # Custom React hooks
│   │   ├── utils/           # Utility functions
│   │   ├── styles/          # CSS/Tailwind
│   │   └── App.jsx
│   ├── public/              # Static assets
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── routes/          # API routes
│   │   ├── controllers/     # Route controllers
│   │   ├── models/          # Database models
│   │   ├── middleware/      # Express middleware
│   │   ├── utils/           # Utility functions
│   │   ├── config/          # Configuration
│   │   └── server.js
│   ├── tests/               # Test files
│   └── package.json
│
├── docs/                    # Documentation
├── public/                  # Public assets
├── .gitignore
├── .env.example
├── package.json             # Root package.json
├── README.md
└── CONTRIBUTING.md
```

## Frontend Structure

The frontend is built with React and Vite for fast development.

### Key Directories

- **components/**: Reusable React components (Button, Card, Restaurant, etc.)
- **pages/**: Full page components (Home, Orders, Profile, etc.)
- **services/**: API client services for backend communication
- **hooks/**: Custom React hooks for logic reuse
- **utils/**: Helper functions and utilities
- **styles/**: Tailwind CSS and global styles

## Backend Structure

The backend is built with Node.js and Express.js.

### Key Directories

- **routes/**: API route definitions
- **controllers/**: Business logic for routes
- **models/**: MongoDB schema definitions
- **middleware/**: Authentication, error handling, etc.
- **utils/**: Helper functions and database utilities
- **config/**: Environment and database configuration

## Environment Setup

Copy `.env.example` to `.env` and configure:

```bash
cp .env.example .env
```

## Getting Started

1. Install dependencies: `npm install`
2. Configure environment: `cp .env.example .env`
3. Start development servers: `npm run dev`
4. Frontend runs on http://localhost:3000
5. Backend runs on http://localhost:5000
