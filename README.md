# Laravelte

**Laravelte** is a lightweight boilerplate combining **Laravel**, **Svelte**, **TypeScript**, **TailwindCSS**, **Vite**, and **Pest** testing—designed to help you build applications with modern tooling, frontend/backend separation, and great developer experience.

---

## Overview

- **Frameworks & Languages**
  - Laravel (backend PHP framework)
  - Svelte (frontend component framework)
  - TypeScript (typed JavaScript)
- **UI & Tooling**
  - TailwindCSS for utility-first styling
  - Vite as fast build & dev tooling
- **Testing & CI**
  - PestPHP for expressive testing
  - GitHub Actions configured via `.github/workflows`
- **Other Features**
  - A clean project structure (`app/`, `resources/`, `routes/`, `tests/`, etc.)
  - Dev tool configurations (ESLint, Prettier, Bun or npm/Yarn)

---

## Table of Contents

1. [Features](#features)  
2. [Installation](#installation)  
3. [Development](#development)  
4. [Testing](#testing)  
5. [Deployment](#deployment)  
6. [Contributing](#contributing)  
7. [License](#license)

---

## Features

- Full-stack scaffolding using Laravel and Svelte
- Modern frontend workflow powered by Vite and TypeScript
- Rapid styling using TailwindCSS
- Pre-configured testing via PestPHP
- CI/CD pipelines ready with GitHub Actions
- Clean project layout and tooling (ESLint, Prettier)

---

## Installation

```bash
git clone https://github.com/ahmadmuqri0/laravelte.git
cd laravelte
composer install               # Install PHP dependencies
npm install                    # or yarn / bun install
cp .env.example .env           # Copy environment variables
php artisan key:generate       # Generate application key
```

---

## Development

```bash
npm run dev                    # Start Vite for frontend hot-reloading
php artisan serve              # Start backend Laravel server
```

- Visit your app at **http://localhost:8000**
- Update Svelte pages under `resources/js` or the appropriate `resources/` structure.

---

## Testing

```bash
php artisan test               # Run all tests via Pest
php artisan test --group=api   # Run only API tests, if grouped
```

---

## Deployment

```bash
npm run build                  # Build front-end assets with Vite
php artisan migrate            # Run database migrations
php artisan optimize           # Optimize Laravel for production
```

- Serve the application using your preferred method (Apache, Nginx, Docker, etc.)

---

## Contributing

Contributions are welcome! Please ensure your changes follow the project style guidelines (Prettier, ESLint), include tests where appropriate, and run all checks before opening a pull request.

---

## License

This project is open-source and available under the **MIT License**.
