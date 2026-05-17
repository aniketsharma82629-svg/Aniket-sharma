# Ewaste Management LMT.

Local-first full-stack e-waste management platform built with Next.js, TypeScript, Tailwind CSS, Prisma Client, and SQLite.

## What it includes

- Customer registration and login
- Shop owner registration with admin approval workflow
- Admin dashboard for approvals, complaints, and review moderation
- GPS location support with manual city fallback
- Nearby authorized shop discovery
- Ratings, reviews, and complaint tracking
- Rental catalog with local checkout flow
- Repair booking and resale request flows
- Local-only data storage in SQLite

## Tech stack

- Next.js 16
- React 19
- TypeScript
- Tailwind CSS 4
- Prisma Client
- SQLite

## Local setup

1. Install dependencies:

```bash
npm install
```

2. Generate the Prisma client:

```bash
npx prisma generate
```

3. Create the local SQLite schema:

```bash
npm run db:setup
```

4. Seed demo data:

```bash
npm run db:seed
```

5. Start the app:

```bash
npm run dev
```

6. Open:

```text
http://localhost:3000
```

## Demo accounts

- Admin: `admin@ewaste.in` / `Admin@123`
- Customer: `riya@ewaste.in` / `Customer@123`
- Shop owner: `aarav@greengrid.in` / `Owner@123`

## Data location

- Main local database: `prisma/dev.db`
- Environment config: `.env`

## Validation completed

- `npm run lint`
- `npm run build`

## Main routes

- `/`
- `/register`
- `/login`
- `/dashboard`
- `/shops`
- `/rentals`
- `/repair`
- `/resale`
- `/history`
- `/profile`
- `/owner`
- `/admin`
