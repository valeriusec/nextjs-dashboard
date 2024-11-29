# Nextjs Acme Dashboard

This project is a dashboard application built with Next.js, utilizing the App Router feature. It includes various functionalities such as invoice management, customer management, and authentication.

## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Scripts](#scripts)

## Features

- Invoice management (create, edit, search, and paginate invoices)
- Customer management (search and display customers)
- Authentication with NextAuth
- Responsive design with Tailwind CSS

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository:

   ```sh
   git clone https://github.com/valeriusec/nextjs-dashboard.git
   cd acme-dashboard
   ```

2. Install dependencies:

   ```sh
   pnpm install
   ```

3. Create a .env file based on the .env.example file and configure your environment variables.

4. Run the development server:

```sh
   pnpm dev
```

5. Open your browser and navigate to <http://localhost:3000>.

## Project Structure

```bash
.env
.eslintrc.json
.gitignore
.next/
app/
    ├── dashboard/
    │   ├── invoices/
    │   │   ├── page.tsx
    │   │   └── [id]/
    │   │       └── edit/
    │   │           └── page.tsx
    │   ├── customers/
    │       └── page.tsx
    ├── ui/
    │   ├── search.tsx
    │   ├── invoices/
    │   │   ├── table.tsx
    │   │   ├── pagination.tsx
    │   │   ├── edit-form.tsx
    │   │   └── create-form.tsx
    │   ├── customers/
    │       └── table.tsx
    ├── lib/
    │   ├── actions.ts
    │   ├── data.ts
    │   └── definitions.ts
auth.config.ts
auth.ts
middleware.ts
next-env.d.ts
next.config.ts
package.json
pnpm-lock.yaml
postcss.config.js
public/
README.md
tailwind.config.ts
tsconfig.json
```

## Scripts

- `pnpm build`: Build the project
- `pnpm dev`: Run the development server
- `pnpm start`: Start the production server
- `pnpm lint`: Run ESLint
