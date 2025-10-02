# Next.js Dashboard App

A starter dashboard application built with [Next.js](https://nextjs.org/) App Router, TypeScript, Tailwind CSS, and modern best practices. This project is designed as a learning resource and template for building full-stack React applications.

## Features

- **Next.js App Router**: Uses the latest Next.js routing features.
- **TypeScript**: Type-safe codebase.
- **Tailwind CSS**: Utility-first CSS framework for rapid UI development.
- **Authentication**: Ready for integration with [next-auth](https://next-auth.js.org/).
- **PostgreSQL Integration**: Uses the `postgres` package for database access.
- **Component-based UI**: Reusable components and skeleton loaders.
- **Responsive Design**: Mobile and desktop layouts.
- **Modern Tooling**: ESLint, Prettier, and more.
- **Server Actions**: Uses Next.js [Server Actions](https://nextjs.org/docs/app/building-your-application/data-fetching/server-actions) for form handling.
- **Accessible Forms**: Forms include proper labels, error handling, and ARIA attributes.

## Project Structure

```
.
├── app/                  # Main application routes and components
│   ├── dashboard/        # Dashboard pages, logic, and UI
│   ├── ui/               # Reusable UI components (e.g., AcmeLogo, skeletons, forms)
│   │   └── invoices/     # Invoice-related UI components (e.g., create-form.tsx)
│   ├── lib/              # Utility functions, server actions, and data fetching logic
│   └── page.tsx          # Landing page
├── public/               # Static assets (images, favicon, etc.)
├── styles/               # Global styles (if any)
├── tailwind.config.ts    # Tailwind CSS configuration
├── postcss.config.js     # PostCSS configuration
├── next.config.ts        # Next.js configuration
├── package.json          # Project metadata and scripts
├── tsconfig.json         # TypeScript configuration
└── README.md             # Project documentation
```

## Getting Started

### Prerequisites

- Node.js 18+
- [pnpm](https://pnpm.io/) (or npm/yarn)

### Installation

```sh
pnpm install
```

### Development

```sh
pnpm dev
```

### Production Build

```sh
pnpm build
pnpm start
```

### Linting

```sh
pnpm lint
```

## Environment Variables

Copy `.env.example` to `.env` and fill in required values.

## Scripts

- `dev`: Start development server
- `build`: Build for production
- `start`: Start production server
- `lint`: Run ESLint

## Key Technologies

- [Next.js](https://nextjs.org/)
- [React](https://react.dev/)
- [Tailwind CSS](https://tailwindcss.com/)
- [PostgreSQL](https://www.postgresql.org/) (via [`postgres`](https://github.com/porsager/postgres))
- [next-auth](https://next-auth.js.org/)
- [clsx](https://github.com/lukeed/clsx)
- [@heroicons/react](https://github.com/tailwindlabs/heroicons)
- [zod](https://zod.dev/)

## Notes

- **Forms**: The app uses [Server Actions](https://nextjs.org/docs/app/building-your-application/data-fetching/server-actions) for form submissions (see `app/ui/invoices/create-form.tsx` and `app/lib/actions.ts`). Ensure your Next.js version supports this feature.
- **Accessibility**: Forms include ARIA attributes and error messaging for improved accessibility.
- **Customization**: Update the `app/ui/` and `app/lib/` directories to add or modify UI and business logic.

## Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [Course Curriculum](https://nextjs.org/learn)

---
