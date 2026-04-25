# AIautomationtools2026

Digital product built by Agency AI

## Tech Stack
- Framework: Next.js 14 (App Router) + TypeScript + TailwindCSS
- Database: Supabase (Postgres + Auth + Storage) — free tier
- Hosting: Vercel (free tier, auto-SSL, CI/CD из GitHub)
- Payments: Stripe Checkout (hosted page, no PCI scope) + Stripe Webhooks

## Quick Start
```bash
npm install
git push origin main && vercel --prod  # Vercel auто-собирает из GitHub; env vars (ANTHROPIC_API_KEY, SUPABASE_*, STRIPE_*) выставлены через `vercel env add` заранее
```

## Core Feature
AI Workflow Generator: Пользователь описывает задачу обычным языком ('каждый день в 9 утра брать новые письма из Gmail с темой Invoice, парсить сумму и сохранять в Google Sheets'), получает готовый JSON-workflow для n8n/Zapier с пошаговыми инструкциями импорта. Один Claude API вызов = один готовый рабочий automation.

---
Built automatically by [Agency AI Business Factory](https://github.com/aisymbioz-gif)
