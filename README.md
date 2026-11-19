# Hi, I'm Rodion Ramazanov 👋

[Telegram @iamrodionn](https://t.me/iamrodionn) · [rodion.rm111@icloud.com](mailto:rodion.rm111@icloud.com) · [GitHub @FatB0YY](https://github.com/FatB0YY)

**Fullstack Developer & LLM Engineer**

I build React and TypeScript frontends and Node.js APIs with Express and NestJS. My web work includes frontend architecture, performance and third-party integrations.

**I work on LLM inference and model serving, and I’m interested in retrieval-augmented generation (RAG) and agents that use external tools. I plan to share code walkthroughs on reducing inference latency, measuring retrieval quality, and testing how reliably agents choose and use tools.**

## Under the hood

Mechanisms that usually stay hidden inside a framework or runtime, rebuilt from scratch or taken apart to show how they actually work.

- **[custom-rendering-strategies](https://github.com/FatB0YY/custom-rendering-strategies)** — CSR, App Shell, SSG, partial SSG, ISR, SSR, streaming SSR and SSI **implemented without a framework**: the low-level mechanics Next.js hides.
- **[yieldpoint-cooperative-scheduler](https://github.com/FatB0YY/yieldpoint-cooperative-scheduler)** — Cooperative multitasking in TypeScript with zero dependencies: generator tasks mark their own yield points, and a round-robin scheduler pauses them on one shared time budget. The machinery behind React's scheduler and `scheduler.yield()`.
- **[sync-promise](https://github.com/FatB0YY/sync-promise)** — A Promise-like **finite-state machine** that runs handlers synchronously, without queuing microtasks.
- **[react-compiler-under-the-hood](https://github.com/FatB0YY/react-compiler-under-the-hood)** — What React Compiler actually emits for a React 19 component, side by side with the hand-memoized version. The annotated compiler output shows the cache slots, sentinel checks and guards that replace hand-written `useMemo`, `useCallback` and `memo`.

## Integrations & production solutions

Problems that come up in real products — authentication flows, third-party widgets, embedding an app into a page you don't control.

- **[auth-demo-httpOnly-cookies](https://github.com/FatB0YY/auth-demo-httpOnly-cookies)** — JWT auth on **httpOnly cookies**: an Axios interceptor with silent token refresh and a request queue, TanStack Router route guards, a redirect-loop guard, and the backend contract it relies on.
- **[third-party-auth-integration](https://github.com/FatB0YY/third-party-auth-integration)** — An external provider owns the user's identity while the application backend owns the session. The Next.js app exchanges provider tokens for a backend session, refreshes them and chains middleware to guard private routes.
- **[iframe-react-integration](https://github.com/FatB0YY/iframe-react-integration)** — Moving one iframe between Tilda popups keeps the embedded Next.js app mounted. A `MutationObserver` tracks host changes, `requestAnimationFrame` batches updates and the `postMessage` handlers validate the sender's origin.
- **[cloudpayments-react-integration](https://github.com/FatB0YY/cloudpayments-react-integration)** — **CloudPayments PaymentBlocks** in Next.js App Router. The form mounts the widget in the browser, shows a fallback if the script is blocked, and cleans up on unmount. Payment and fiscal receipt data are typed.

## Full-stack applications

- **[BIKE_FORCE](https://github.com/FatB0YY/BIKE_FORCE)** — A server-rendered bicycle store and a React admin panel share an Express API and a normalized PostgreSQL schema to 3NF. RTK Query handles catalog updates.
- **[CLOUD-STORAGE](https://github.com/FatB0YY/CLOUD-STORAGE)** — A React file browser with uploads, nested folders and file search. An Express API handles file operations and stores metadata in MongoDB.
- **[SQUAD](https://github.com/FatB0YY/SQUAD)** — A Next.js collaboration app with channels, membership roles and file sharing. It uses Auth.js and Prisma with PostgreSQL and includes a Socket.IO chat server.

## Frontend applications

- **[MIDDLE-PROJECT](https://github.com/FatB0YY/MIDDLE-PROJECT)** — Production-grade React article platform with a custom ESLint plugin that enforces Feature-Sliced Design boundaries. Storybook, component tests, visual regression tests and feature flags support UI changes, i18n and CI.
- **[MFE-PEOPLE-HUB](https://github.com/FatB0YY/MFE-PEOPLE-HUB)** — A Module Federation host loads two React micro-frontends independently. They share profile updates through typed events, and one can keep working when the other fails to load.

## React 19: hooks and new APIs

- **[react-custom-hooks](https://github.com/FatB0YY/react-custom-hooks)** — 14 hooks covering stable callbacks, DOM event subscriptions, ref composition, frame throttling and resize observation.
- **[react19-new-hooks](https://github.com/FatB0YY/react19-new-hooks)** — `use`, `useActionState`, `useOptimistic`, `useTransition`, `useDeferredValue`, `useEffectEvent` and the new `createRoot` error options, each shown as before vs after.
