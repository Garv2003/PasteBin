# PasteBin

> **Status: initialized, not yet implemented.** This repository currently contains only a freshly generated Next.js starter application. None of the pastebin functionality (creating, storing, or viewing text snippets) has been built yet. The name reflects the intended direction of the project, not its current capabilities.

## Overview

PasteBin is intended to become a text/snippet sharing application. At present the repo holds a single `client/` directory containing an unmodified `create-next-app` scaffold (Next.js 15, App Router, React 19, TypeScript, Tailwind CSS). The landing page is the default Next.js template ("Get started by editing `src/app/page.tsx`", with the standard Vercel/Next.js links). There is no backend, no data storage, no API routes, and no paste-related UI in the codebase.

## Current state (honest scope)

- `client/src/app/page.tsx` is the stock create-next-app landing page.
- `client/src/app/layout.tsx` and `globals.css` are the default scaffold files.
- No server, database, or persistence layer exists.
- No paste creation, snippet, syntax-highlighting, or expiry features are implemented — do not assume any of these are present.

In short, this is a clean starting point ready for feature development, not a working pastebin.

## Planned features (not yet built)

Based on the project name, the likely intended scope is creating and sharing text snippets. None of this is implemented today; it is listed only to describe direction.

## Tech stack

From `client/package.json`:
- **Next.js 15** (App Router, Turbopack dev server)
- **React 19** / React DOM 19
- **TypeScript 5**
- **Tailwind CSS 3** (+ PostCSS)
- **ESLint 9** with `eslint-config-next`

## Getting started

```bash
cd client
pnpm install       # a pnpm-lock.yaml is checked in
pnpm dev           # start the Next.js dev server (http://localhost:3000)
```

Other scripts (from `package.json`):
```bash
pnpm build         # production build
pnpm start         # serve the production build
pnpm lint          # run ESLint
```

## Usage

Running `pnpm dev` serves the default Next.js starter page. There is currently no pastebin functionality to use. Development would begin by replacing the boilerplate in `client/src/app/page.tsx` and adding the necessary routes, UI, and storage.

## Project structure

```
PasteBin/
└── client/                     # Next.js 15 starter (unmodified create-next-app)
    ├── package.json            # next 15, react 19, tailwind, eslint
    ├── next.config.ts
    ├── tailwind.config.ts
    ├── postcss.config.mjs
    ├── eslint.config.mjs
    ├── tsconfig.json
    ├── public/                 # default Next.js SVG assets
    └── src/app/
        ├── layout.tsx          # default starter layout
        ├── page.tsx            # default create-next-app landing page
        └── globals.css         # default global styles
```
