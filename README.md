# TanStack Start Application

A modern, full-stack React application built with [TanStack Start](https://tanstack.com/start). Designed for type-safe routing, server-side rendering, and a polished developer experience.

## Tech Stack

- **Framework:** [TanStack Start v1](https://tanstack.com/start) — full-stack React with SSR/SSG and server functions
- **Build Tool:** [Vite 8](https://vitejs.dev/) for fast development and production builds
- **UI Library:** [React 19](https://react.dev/)
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com/) with CSS theme variables and `oklch` tokens
- **Components:** [shadcn/ui](https://ui.shadcn.com/) primitives built on [Radix UI](https://www.radix-ui.com/)
- **State & Data:** [TanStack Query](https://tanstack.com/query) for server-state management
- **Routing:** [TanStack Router](https://tanstack.com/router) with file-based route generation
- **Forms & Validation:** [React Hook Form](https://react-hook-form.com/) + [Zod](https://zod.dev/)
- **Icons:** [Lucide React](https://lucide.dev/)
- **Charts:** [Recharts](https://recharts.org/)
- **Notifications:** [Sonner](https://sonner.emilkowal.ski/)

## Features

- File-based routing with automatic route tree generation
- Type-safe server functions via `createServerFn`
- SSR-ready shell layout in `src/routes/__root.tsx`
- Dark mode tokens ready via `oklch` CSS variables
- Pre-configured ESLint + Prettier for consistent code style
- shadcn/ui components available under `src/components/ui/`

## Quick Start

1. **Install dependencies**

   ```bash
   bun install
   ```

2. **Start the development server**

   ```bash
   bun dev
   ```

3. **Open the app**

   Navigate to [http://localhost:8080](http://localhost:8080).

## Available Scripts

| Script         | Description                              |
| -------------- | ---------------------------------------- |
| `bun dev`      | Start the development server             |
| `bun build`    | Build for production                     |
| `bun build:dev`| Build in development mode                |
| `bun preview`  | Preview the production build locally     |
| `bun lint`     | Run ESLint across the project            |
| `bun format`   | Format files with Prettier               |

## Project Structure

```text
src/
├── components/ui/      # shadcn/ui components
├── hooks/              # Reusable React hooks
├── lib/                # Utilities and helpers
├── routes/             # TanStack file-based routes
│   ├── __root.tsx      # Root layout with providers
│   └── index.tsx       # Home page
├── server.ts           # Server configuration
├── start.ts            # Application startup
└── styles.css          # Tailwind theme tokens
```

## Conventions

- Routes are defined in `src/routes/` using the [TanStack Router file convention](https://tanstack.com/router/latest/docs/framework/react/routing/file-based-routing).
- Server functions are created with `createServerFn` from `@tanstack/react-start`.
- Colors and themes use semantic CSS tokens in `src/styles.css`; avoid hardcoded hex values in components.
- Import UI components from `@/components/ui/<component>`.

## Resources

- [TanStack Start Docs](https://tanstack.com/start/latest/docs/framework/react/overview)
- [TanStack Router Docs](https://tanstack.com/router/latest/docs/framework/react/overview)
- [Tailwind CSS v4 Docs](https://tailwindcss.com/docs/v4-beta)
- [shadcn/ui Docs](https://ui.shadcn.com/docs)

---

Built with [Lovable](https://lovable.dev).
