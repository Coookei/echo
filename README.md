# Echo Monorepo Experiment

This is an experimental project for learning how to build a clean, modular monorepo powered by Next.js sites and TurboRepo. The goal is to explore how apps, shared packages, and UI modules can live together with a tidy project structure to provide a smooth developer experience.

## What we're trying out

- Next.js apps that share code via internal packages
- Reusable UI modules inspired by the shadcn/ui approach
- Consistent TurboRepo pipelines for linting, formatting, and testing across the workspace

## Getting started

```bash
pnpm install
pnpm dev
```

## Adding UI components

Run component generators from the root of the `web` app to keep shared pieces in `packages/ui`:

```bash
pnpm dlx shadcn@latest add button -c apps/web
```

## Useful commands

```bash
pnpm dev      # runs all apps and modules through TurboRepo with hot reloading
pnpm build    # build every package/app in the workspace
pnpm lint     # run lint checks across the repo with shared configs
```
