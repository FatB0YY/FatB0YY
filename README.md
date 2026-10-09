# Hi, I'm **Rodion Ramazanov** 👋

### Connect

* Telegram: [@iamrodionn](https://t.me/iamrodionn)
* Email: [rodion.rm111@icloud.com](mailto:rodion.rm111@icloud.com)
* GitHub: [FatB0YY](https://github.com/FatB0YY)

**Full-stack Engineer**

Building production-grade web applications with **React, TypeScript, and Node.js**.

I focus on frontend architecture, performance, developer experience, and structured AI-assisted engineering workflows with **Claude Code**.

### Under the hood

Mechanisms that usually stay hidden inside a framework or runtime, rebuilt from scratch or taken apart to show how they actually work.

* **[custom-rendering-strategies](https://github.com/FatB0YY/custom-rendering-strategies)** — CSR, App Shell, SSG, partial SSG, ISR, SSR, streaming SSR and SSI implemented without a framework: the low-level mechanics Next.js hides.
* **[yieldpoint-cooperative-scheduler](https://github.com/FatB0YY/yieldpoint-cooperative-scheduler)** — Cooperative multitasking in TypeScript with zero dependencies: generator tasks mark their own yield points, and a round-robin scheduler pauses them on one shared time budget. The machinery behind React's scheduler and `scheduler.yield()`.
* **[sync-promise](https://github.com/FatB0YY/sync-promise)** — A Promise-like implementation that runs handlers synchronously, without microtasks: state machine, chaining, error propagation, thenable assimilation and self-resolution protection.
* **[react-compiler-under-the-hood](https://github.com/FatB0YY/react-compiler-under-the-hood)** — What React Compiler actually emits for a React 19 component: cache slots, sentinel checks and per-node guards that replace `memo()`, next to the hand-written `useMemo` / `useCallback` / `memo` version.
* **[type-challenges-solutions](https://github.com/FatB0YY/type-challenges-solutions)** — TypeScript's built-in utilities (`Pick`, `Readonly`, `Exclude`, `Parameters`, `ReturnType`) reimplemented at the type level, plus tuple manipulation, each with an explanation.

### Integrations & production solutions

Problems that come up in real products — authentication flows, third-party widgets, embedding an app into a page you don't control — and how they were solved.

* **[auth-demo-httpOnly-cookies](https://github.com/FatB0YY/auth-demo-httpOnly-cookies)** — JWT auth on httpOnly cookies: an Axios interceptor with silent token refresh and a request queue, TanStack Router route guards, a redirect-loop guard, and the backend contract it relies on.
* **[third-party-auth-integration](https://github.com/FatB0YY/third-party-auth-integration)** — Authentication against an external provider in Next.js: token acquisition and refresh, session exchange with a first-party backend, and a composable middleware chain for private routes.
* **[iframe-react-integration](https://github.com/FatB0YY/iframe-react-integration)** — Embedding a Next.js app into a website-builder page you don't control: one iframe relocated between popup slots instead of recreated, popup state detection via `MutationObserver` with rAF batching, and a two-way `postMessage` protocol with origin validation.
* **[cloudpayments-react-integration](https://github.com/FatB0YY/cloudpayments-react-integration)** — The CloudPayments payment widget in Next.js App Router: external script loading, mount/unmount lifecycle, SSR guards, blocked-script handling, typed init params and fiscal receipt data.

### Frontend & full-stack applications

Complete applications, from frontend architecture and testing to APIs, databases and infrastructure.

* **[MIDDLE-PROJECT](https://github.com/FatB0YY/MIDDLE-PROJECT)** — Production-grade React article platform: Feature-Sliced Design enforced by a custom ESLint plugin, unit / component / visual regression tests, Storybook, i18n, feature flags with automated cleanup, dual Webpack + Vite builds and CI.
* **[BIKE_FORCE](https://github.com/FatB0YY/BIKE_FORCE)** — Full-stack bicycle store: Express + TypeScript API over a PostgreSQL schema normalised to 3NF, server-side rendered storefront, React + RTK Query admin panel, nginx and Docker Compose.
* **[CLOUD-STORAGE](https://github.com/FatB0YY/CLOUD-STORAGE)** — Google Drive-style file storage: React + RTK Query client, Express + MongoDB API, JWT access/refresh tokens with silent refresh via Axios interceptors, nested folders and search.
* **[SQUAD](https://github.com/FatB0YY/SQUAD)** — Team collaboration app on Next.js App Router: servers, channels, real-time messaging and file sharing, with Auth.js OAuth, Prisma + serverless Postgres, typed i18n, Zod validation and Sentry.
* **[MEHN-stack_coursesApp](https://github.com/FatB0YY/MEHN-stack_coursesApp)** — Server-rendered course marketplace on MongoDB, Express, Handlebars and Node.js: session-cookie auth, CSRF protection, route guards, email password reset and server-side validation.

### React: hooks and new APIs

Reusable hooks for everyday problems and a hands-on look at what React 19 changes.

* **[react-custom-hooks](https://github.com/FatB0YY/react-custom-hooks)** — 14 custom hooks: stable callbacks, leak-free event subscriptions, debounce and rAF throttling, ref composition, resize observation. Each one is documented and comes with a usage example.
* **[react19-new-hooks](https://github.com/FatB0YY/react19-new-hooks)** — `use`, `useActionState`, `useOptimistic`, `useTransition`, `useDeferredValue`, `useEffectEvent` and the new `createRoot` error options, each shown as before vs after with both versions running live.
