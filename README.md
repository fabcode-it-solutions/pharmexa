# Pharmexa

Pharmexa is a full-stack pharmacy platform: a customer-facing storefront for browsing products, ordering, and managing prescriptions, plus an admin centre for managing products, orders, prescriptions, categories, blog content, and pharmacy settings.

**Repository:** https://github.com/fabcode-it-solutions/pharmexa

## Project structure

```
.
├── backend/    # Express + Prisma API (PostgreSQL via Supabase)
└── frontend/   # React + TypeScript + Vite storefront and admin UI
```

## Tech stack

- **Frontend:** React 19, TypeScript, Vite, Tailwind CSS, React Router, React Hook Form, Zod
- **Backend:** Express 5, Prisma ORM, PostgreSQL, JWT auth, bcrypt, Zod

## Getting started

### Backend

```bash
cd backend
npm install
npm run dev
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

Each package manages its own environment variables and Prisma/database setup — see `backend/prisma/schema.prisma` for the data model.

## Scripts

| Location | Command | Purpose |
| --- | --- | --- |
| `backend` | `npm run dev` | Start the API in watch mode |
| `backend` | `npm run build` | Compile TypeScript |
| `backend` | `npm start` | Run the compiled API |
| `frontend` | `npm run dev` | Start the Vite dev server |
| `frontend` | `npm run build` | Type-check and build for production |
| `frontend` | `npm run lint` | Run ESLint |
