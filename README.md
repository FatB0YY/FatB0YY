# Hi, I'm Rodion Ramazanov 👋

[Telegram @iamrodionn](https://t.me/iamrodionn) · [rodion.rm111@icloud.com](mailto:rodion.rm111@icloud.com) · [GitHub @FatB0YY](https://github.com/FatB0YY)

**Full-stack Developer & LLM Engineer**

I build React and TypeScript frontends and Node.js APIs with Express and NestJS. My web work includes frontend architecture, performance and third-party integrations.

My LLM work focuses on inference. I plan to publish code walkthroughs showing how tokenization, attention and decoding turn a prompt into generated text.

## Under the hood

I rebuild parts of frameworks and runtimes to understand the decisions they usually make for me.

- **[custom-rendering-strategies](https://github.com/FatB0YY/custom-rendering-strategies)** — CSR, App Shell, SSG, partial SSG, ISR, SSR, streaming SSR and SSI implemented without Next.js. The examples show when HTML is built, when a cached page is regenerated and when the browser receives the first chunk.
- **[yieldpoint-cooperative-scheduler](https://github.com/FatB0YY/yieldpoint-cooperative-scheduler)** — Dependency-free cooperative multitasking in TypeScript. Generator tasks mark their yield points, and a round-robin scheduler uses a shared time budget to decide when to return control to the event loop.
- **[sync-promise](https://github.com/FatB0YY/sync-promise)** — A Promise-like state machine that runs handlers synchronously, without queuing microtasks. Tests cover chaining, error propagation, thenable assimilation and self-resolution.
- **[react-compiler-under-the-hood](https://github.com/FatB0YY/react-compiler-under-the-hood)** — One React 19 component written with and without manual memoization. The annotated compiler output shows the cache slots, sentinel checks and guards that replace hand-written `useMemo`, `useCallback` and `memo`.

## Integrations & production solutions

- **[auth-demo-httpOnly-cookies](https://github.com/FatB0YY/auth-demo-httpOnly-cookies)** — When several API calls receive a 401 at once, an Axios interceptor queues them behind one token refresh and replays them. The demo includes HttpOnly cookies, TanStack Router guards and redirect-loop handling.
- **[third-party-auth-integration](https://github.com/FatB0YY/third-party-auth-integration)** — An external provider owns the user's identity while the application backend owns the session. The Next.js app exchanges provider tokens for a backend session, refreshes them and chains middleware to guard private routes.
- **[iframe-react-integration](https://github.com/FatB0YY/iframe-react-integration)** — Moving one iframe between Tilda popups keeps the embedded Next.js app mounted. A `MutationObserver` tracks host changes, `requestAnimationFrame` batches updates and the `postMessage` handlers validate the sender's origin.
- **[cloudpayments-react-integration](https://github.com/FatB0YY/cloudpayments-react-integration)** — CloudPayments PaymentBlocks in Next.js App Router. The form mounts the widget in the browser, shows a fallback if the script is blocked, and cleans up on unmount. Payment and fiscal receipt data are typed.

## Full-stack applications

- **[BIKE_FORCE](https://github.com/FatB0YY/BIKE_FORCE)** — A server-rendered bicycle store and a React admin panel share an Express API and a normalized PostgreSQL schema. RTK Query handles catalog updates.
- **[CLOUD-STORAGE](https://github.com/FatB0YY/CLOUD-STORAGE)** — A React file browser with uploads, nested folders and file search. An Express API handles file operations and stores metadata in MongoDB.
- **[SQUAD](https://github.com/FatB0YY/SQUAD)** — A Next.js collaboration app with channels, membership roles and file sharing. It uses Auth.js and Prisma with PostgreSQL and includes a Socket.IO chat server.

## Frontend applications

- **[MIDDLE-PROJECT](https://github.com/FatB0YY/MIDDLE-PROJECT)** — A React article platform with a custom ESLint plugin that enforces Feature-Sliced Design boundaries. Storybook, component tests, visual regression tests and feature flags support UI changes.
- **[MFE-PEOPLE-HUB](https://github.com/FatB0YY/MFE-PEOPLE-HUB)** — A Module Federation host loads two React micro-frontends independently. They share profile updates through typed events, and one can keep working when the other fails to load.

## React & TypeScript practice

- **[react-custom-hooks](https://github.com/FatB0YY/react-custom-hooks)** — 14 hooks covering stable callbacks, DOM event subscriptions, ref composition, frame throttling and resize observation.
- **[react19-new-hooks](https://github.com/FatB0YY/react19-new-hooks)** — Side-by-side demos of React 19 APIs, including `useActionState`, `useOptimistic` and `useEffectEvent`. Each example displays the source it actually runs.

For fun, I also solve [TypeScript type challenges](https://github.com/FatB0YY/type-challenges-solutions), like building a fixed-length tuple using only types.
