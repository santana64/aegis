# Aegis - Monorepo SaaS Full-Stack

Architecture monorepo de reference pour SaaS modernes. Backend REST Fastify, frontend Next.js, SDK TypeScript publiable, packages partages. Orchestration Turborepo.

## Architecture

bash
aegis/
  apps/
    backend/    # API REST Fastify + Prisma + PostgreSQL
    frontend/   # Next.js 14 App Router
  packages/
    config/     # ESLint, TypeScript, Tailwind configs partages
    sdk-ts/     # SDK TypeScript consommable par clients externes
    shared/     # Types et utilitaires partages
  turbo.json
  pnpm-workspace.yaml


## Stack

| Couche | Technologie |
|---|---|
| Backend | Fastify + @fastify/cors |
| ORM | Prisma + pg adapter |
| Base de donnees | PostgreSQL |
| Frontend | Next.js 14 |
| SDK | TypeScript (publishable) |
| Orchestration | Turborepo + pnpm workspaces |
| Validation | Zod |

## Fonctionnalites

- API REST typee et documentee (Fastify)
- Frontend consommant l API via le SDK interne
- SDK TypeScript isomorphe publiable sur npm
- Configuration ESLint et TypeScript partagee
- Build parallele optimise via Turborepo
- Pipeline CI/CD pret a l emploi

## Demarrage

bash
npm install -g pnpm
pnpm install
pnpm run dev
