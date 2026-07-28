<div align="center">

# Igor Vuta

**Software developer — Python · TypeScript · FastAPI · Next.js**

First-Class BSc (Hons) Computer Science · De Montfort University, Leicester, UK

[![Portfolio](https://img.shields.io/badge/Portfolio-igor--vuta.github.io-C15F3C?style=for-the-badge&logo=github&logoColor=white)](https://igor-vuta.github.io/portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-igor--vuta-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/igor-vuta-b88017390)
[![Email](https://img.shields.io/badge/Email-igor__vuta%40proton.me-6D4AFF?style=for-the-badge&logo=protonmail&logoColor=white)](mailto:igor_vuta@proton.me)

</div>

---

## Hi 👋

I write backends and the web apps that sit on top of them, and I have an unreasonable soft spot for the part most people skip: proving the thing actually works.

A benchmark from a single run tells you almost nothing — change the seed and it can tell you the opposite. So when I claim my optimiser beats a greedy baseline, that number comes from 120 scenarios × 30 seeds, reported as a mean with the spread next to it. A result without a distribution is just an anecdote with good lighting.

That habit came out of my degree and never left. Give me a dataset and I'll happily lose an evening to it.

## What I've been building

### Intelli-Factory — final-year project

A supply-chain matching platform: FastAPI + PostgreSQL backend running an **NSGA-II genetic algorithm** (DEAP), with a Next.js/TypeScript frontend.

The interesting part isn't the stack, it's the trade-off. Cost, delivery time and reliability all pull against each other, so there's no single "best" answer — you get a Pareto front and then have to decide what you're actually optimising for. Measured over **3,600 evaluations** (120 scenarios × 30 seeds) against the production engine code:

| Metric | Greedy baseline | Optimised | Change |
|---|---|---|---|
| Composite fitness | 0.682 | 0.801 | **+17.5%** |
| Delivery time | 8.02 days | 4.67 days | **41.8% faster** |
| Reliability | 0.824 | 0.891 | **+8.1%** |
| Raw cost | 21,296 KZT | 51,648 KZT | +142.5% — a deliberate trade |

Pareto-front hypervolume **0.852 ± 0.12**, converging around generations 50–60. Feasibility **100%** across every scenario. Response time **0.069 s ± 0.015 s**. Runs are seeded, so the numbers reproduce.

Also 51 pytest tests (TDD on the engine) and OWASP-aligned security — Argon2id, server-side sessions, rate limiting.

**[Live demo](https://intelli-factory-frontend.vercel.app/)** · **[API docs](https://intelli-factory-api.onrender.com/docs)** · **[Code](https://github.com/igor-vuta/intelli-factory)**

> Heads up: the API sits on a free tier and falls asleep. Open the register page and give it ~90 seconds to wake up before assuming it's broken.

### Everything else

| Project | What it is | Live |
|---|---|---|
| [portfolio](https://github.com/igor-vuta/portfolio) | Editorial one-pager. Hand-rolled animations, zero UI libraries | [Visit](https://igor-vuta.github.io/portfolio/) |
| [todo-webapp-refactored](https://github.com/igor-vuta/todo-webapp-refactored) | Full-stack task manager — PHP 8.2, MySQL, JWT, shared group lists, Docker | [Visit](https://todo-app-production-5509.up.railway.app/) |
| [drivePro-website](https://github.com/igor-vuta/drivePro-website) | Bilingual (RU/KK) site for an equipment-hire company | [Visit](https://igor-vuta.github.io/drivePro-website/) |
| [currency-exchange-bot](https://github.com/igor-vuta/currency-exchange-bot) | Button-only Telegram bot, API with a scraper fallback | [@currenvy_bot](https://t.me/currenvy_bot_for_demo_bot) |
| [vue-folder-tree](https://github.com/igor-vuta/vue-folder-tree) | Recursive Vue 3 tree component — keyboard nav, ARIA, no dependencies | [Visit](https://igor-vuta.github.io/vue-folder-tree/) |
| [react-starter-pro](https://github.com/igor-vuta/react-starter-pro) | React 19 + Vite starter with the lint/format/hooks/CI boring bits already done | [Visit](https://igor-vuta.github.io/react-starter-pro/) |
| [qubly-landing](https://github.com/igor-vuta/qubly-landing) | Older pixel-perfect landing page. Plain HTML, CSS, jQuery | [Visit](https://igor-vuta.github.io/qubly-landing/) |

## What I reach for

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?logo=tailwindcss&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![pytest](https://img.shields.io/badge/pytest-0A9EDC?logo=pytest&logoColor=white)

Alongside those: DEAP for evolutionary algorithms, pandas and NumPy when I'm poking at data, and Recharts when a result needs to be looked at rather than read.

## Currently

Looking for **entry-level software or web developer roles in the UK**. I'm on the Graduate Route with full-time work rights, so no sponsorship needed.

Certified: Meta Front-End Developer · Palo Alto Cybersecurity Foundation · Red Hat RH124.

If you've got a problem where the right approach isn't obvious and someone needs to measure which one actually wins — that's the job I want.

Reach me at [igor_vuta@proton.me](mailto:igor_vuta@proton.me).
