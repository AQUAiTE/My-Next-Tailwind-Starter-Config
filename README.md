# My Next-Tailwind Starter Config

A personal, ready-to-go configuration base for new **Next.js 15 (App Router)**
projects. This is the config layer only (no application code), so you can drop
your own `app/`, `components/`, and `lib/` on top.

## Stack

- **Next.js 15** + **React 19** + **TypeScript** (strict)
- **Tailwind CSS v4** (`@tailwindcss/postcss`)
- **shadcn/ui** (`components.json` preconfigured, `@/*` path alias)
- **ESLint** flat config: `strictTypeChecked` + `stylisticTypeChecked` + `next`
- **Prettier**: double quotes, semicolons, trailing commas, 2-space, 80 width
- **pnpm** (exact versions, strict peers)

## What's included

| File | Purpose |
| --- | --- |
| `package.json` | scripts + pinned stack dependencies |
| `tsconfig.json` | strict TS, `@/*` alias, bundler resolution |
| `eslint.config.mjs` | flat config, type-checked rules |
| `.prettierrc.json` / `.prettierignore` | formatting style |
| `postcss.config.mjs` | Tailwind v4 plugin |
| `components.json` | shadcn/ui generator config |
| `.npmrc` | pnpm behavior (exact saves, strict peers) |
| `.gitignore` | Next.js + TypeScript ignores |

## Usage

```bash
pnpm install
# add your app/, components/, lib/ and build
pnpm dev
```

## Conventions

- React component files use **TitleCase** (e.g. `Button.tsx`), including
  `components/ui` primitives. Next.js reserved files (`page.tsx`, `layout.tsx`)
  stay lowercase. Non-component modules in `lib/` stay lowercase.
- Path alias `@/*` maps to the project root.
