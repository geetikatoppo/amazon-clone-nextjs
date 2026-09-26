# Contributing

Thank you for your interest in contributing to this project!

## Getting Started

### 1. Fork and clone the repository

Fork this repository on GitHub, then clone your fork to your computer.

### 2. Install dependencies

Run the following command:

```bash
npm install
```

### 3. Configure environment variables

Copy the example environment file:

```bash
cp .env.example .env.local
```

Add the required environment variable values to `.env.local`.

**Important:** Prisma CLI commands such as `prisma generate` and `db:push` read a plain `.env` file, not `.env.local`. If you run Prisma CLI commands directly, make sure your `DATABASE_URL` is also available in `.env`.

### 4. Set up the database

Run:

```bash
npm run db:push
npm run db:seed
```

If MongoDB is unavailable, the application can use the static fallback data in `lib/data.ts`.

### 5. Start the development server

```bash
npm run dev
```

Open the local URL displayed in your terminal.

## Before Opening a Pull Request

Run the project's checks:

```bash
npm run lint
npm run typecheck
```

Make sure your changes do not introduce errors.

## Branch Naming

Create a separate branch for each contribution. Use a short, descriptive name.

Examples:

- `docs/contributing-guide`
- `fix/product-search`
- `feature/shopping-cart`

## Pull Requests

When opening a pull request:

- Explain what you changed.
- Link the related issue when applicable.
- Include screenshots for UI changes.
- Mention important setup or testing details.
- Make sure linting and type checking pass.

Thank you for contributing!
