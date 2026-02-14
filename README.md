# Fullstack React + Fastify + Postgres Template

Starter repository for a fullstack app with:
- `web`: React + Vite frontend served via Nginx
- `api`: Fastify + Prisma backend for PostgreSQL
- `.github/workflows/deploy.yml`: container build and deployment workflow

## Project structure

```
.
├─ web/
├─ api/
├─ .github/workflows/deploy.yml
├─ deploy.config.example.yml
└─ README.md
```

## Quick start

### Web
```bash
cd web
npm install
npm run dev
```

### API
```bash
cd api
npm install
export DATABASE_URL="postgresql://postgres:postgres@localhost:5432/app"
npm run prisma:generate
npm run dev
```

## API endpoints
- `GET /health`
- `GET /db/health`
