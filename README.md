<!-- project-presentation:start -->

![Igor Vuta — Python, TypeScript and the web apps built around them](.github/readme-header.svg)

**[Portfolio](https://igor-vuta.github.io/portfolio/)** · [Repository activity](https://github.com/igor-vuta/igor-vuta/activity)

[![Last commit](https://img.shields.io/github/last-commit/igor-vuta/igor-vuta?style=flat-square&color=6366f1)](https://github.com/igor-vuta/igor-vuta/commits)
[![Repository size](https://img.shields.io/github/repo-size/igor-vuta/igor-vuta?style=flat-square&color=6366f1)](https://github.com/igor-vuta/igor-vuta)

**12** Public repositories · **14** GitHub language categories · **First-class** BSc (Hons) Computer Science

*Project facts checked 2 October 2026. Activity badges update from GitHub.*

<!-- project-presentation:end -->

<div align="center">

First-Class BSc (Hons) Computer Science · De Montfort University, Leicester, UK

[![Portfolio](https://img.shields.io/badge/Portfolio-igor--vuta.github.io-C15F3C?style=for-the-badge&logo=github&logoColor=white)](https://igor-vuta.github.io/portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-igor--vuta-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/igor-vuta)
[![Email](https://img.shields.io/badge/Email-igor__vuta%40proton.me-6D4AFF?style=for-the-badge&logo=protonmail&logoColor=white)](mailto:igor_vuta@proton.me)

<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Activities/Fireworks.png" width="52" alt="fireworks" />
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Animals/Eagle.png" width="52" alt="eagle" />
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Statue%20of%20Liberty.png" width="52" alt="Statue of Liberty" />

*Life, liberty, and the pursuit of reproducible applications.*

</div>

---

## Hi <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Waving%20Hand.png" width="30" alt="waving hand" />

I write backends and the web apps that run on top of them, and I have an unreasonable soft spot for the part most people skip: proving the thing actually works.

A benchmark from a single run tells you almost nothing — change the seed and it can tell you the opposite. So when I claim my optimiser beats a greedy baseline, that number comes from 120 scenarios × 30 seeds, reported as a mean with the spread next to it. A result without a distribution is just an anecdote with good lighting.

That habit came out of my degree and never left. Give me a dataset and I'll happily lose an evening to it.

## What I've been building <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Rocket.png" width="30" alt="rocket" />

### Intelli-Factory — final-year project

A supply-chain matching platform with a **FastAPI + PostgreSQL** backend and a **Next.js/TypeScript** frontend. It ranks manufacturer–logistics offers by a customer-weighted cost, delivery-time and reliability score; a DEAP genetic search cross-checks that score against a greedy cheapest-first baseline.

The interesting part is the trade-off: faster and more reliable offers can cost more. The customer chooses the weights; the deterministic mode exhaustively ranks the available offers, so the genetic search can match that score but cannot improve its optimum. The recorded benchmark covers **3,600 evaluations** (120 scenarios × 30 seeds) against the engine code:

| Metric | Greedy baseline | Optimised | Change |
|---|---|---|---|
| Composite fitness | 0.682 | 0.801 | **+17.5%** |
| Delivery time | 8.02 days | 4.67 days | **41.8% faster** |
| Reliability | 0.824 | 0.891 | **+8.1%** |
| Raw cost | 21,296 KZT | 51,648 KZT | +142.5% — a deliberate trade |

These are recorded benchmark results, not a promise about every real supply chain. The seeded scenarios and exported measurements make the comparison inspectable.

The engine has a pytest regression suite; the application uses Argon2id, server-side sessions and rate limiting. [Recorded benchmark data](https://github.com/igor-vuta/intelli-factory/blob/main/frontend/public/data/benchmark-showcase.json) includes the scenario counts, seeds and measured trade-offs.

**[Live demo](https://intelli-factory.duckdns.org/)** · **[API docs](https://intelli-factory.duckdns.org/api/docs)** · **[Code](https://github.com/igor-vuta/intelli-factory)**

### Applications and tools <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Activities/Sparkles.png" width="26" alt="sparkles" />

| Project | What it is | Live |
|---|---|---|
| [intelli-factory](https://github.com/igor-vuta/intelli-factory) | Weighted supply-chain matching — FastAPI, PostgreSQL, Next.js, DEAP cross-check | [Visit](https://intelli-factory.duckdns.org/) |
| [DrivePro_2](https://github.com/igor-vuta/DrivePro_2) | Navigation-first Almaty carpooling PWA with route-based matching | [Visit](https://drivepro-almaty.duckdns.org/) |
| [portfolio](https://github.com/igor-vuta/portfolio) | Interactive portfolio with a 3D project showcase | [Visit](https://igor-vuta.github.io/portfolio/) |
| [todo-webapp-refactored](https://github.com/igor-vuta/todo-webapp-refactored) | PHP + MySQL task manager with shared lists and JWT authentication | [Run locally](https://github.com/igor-vuta/todo-webapp-refactored#readme) |
| [drivePro-website](https://github.com/igor-vuta/drivePro-website) | Bilingual (RU/KK) site for an equipment-hire company | [Visit](https://igor-vuta.github.io/drivePro-website/) |
| [currency-exchange-bot](https://github.com/igor-vuta/currency-exchange-bot) | Button-only Telegram bot, API with a scraper fallback | [@currenvy_bot](https://t.me/currenvy_bot_for_demo_bot) |
| [vue-folder-tree](https://github.com/igor-vuta/vue-folder-tree) | Recursive Vue 3 tree component — keyboard nav, ARIA, no dependencies | [Visit](https://igor-vuta.github.io/vue-folder-tree/) |
| [react-starter-pro](https://github.com/igor-vuta/react-starter-pro) | React 19 + Vite starter with the lint/format/hooks/CI boring bits already done | [Visit](https://igor-vuta.github.io/react-starter-pro/) |
| [qubly-landing](https://github.com/igor-vuta/qubly-landing) | Older pixel-perfect landing page. Plain HTML, CSS, jQuery | [Visit](https://igor-vuta.github.io/qubly-landing/) |

### Coursework

| Project | What it demonstrates | Try it |
|---|---|---|
| [student-course-hub](https://github.com/igor-vuta/student-course-hub) | Server-rendered course catalogue and admin CMS with Deno, Oak and SQLite | [Local setup](https://github.com/igor-vuta/student-course-hub#readme) |
| [module-chooser-javafx](https://github.com/igor-vuta/module-chooser-javafx) | JavaFX desktop module selection, MVC and credit tracking | [Desktop setup](https://github.com/igor-vuta/module-chooser-javafx#readme) |

## Code at a glance

![Language distribution across public repositories](.github/languages.svg)

*Snapshot: 2 October 2026. GitHub language bytes across public repositories; this shows repository composition, not proficiency or time spent.*

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

## Currently <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Activities/Sparkler.png" width="30" alt="sparkler" />

Looking for **entry-level software and web development roles** where I can build useful applications, learn from experienced engineers and test my work properly.

Certified: Meta Front-End Developer · Palo Alto Cybersecurity Foundation · Red Hat RH124.

If you've got a problem where the right approach isn't obvious and someone needs to measure which one actually wins — that's the job I want.

Reach me at [igor_vuta@proton.me](mailto:igor_vuta@proton.me).

---

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/igor-vuta/igor-vuta/output/github-snake-dark.svg" />
  <img src="https://raw.githubusercontent.com/igor-vuta/igor-vuta/output/github-snake.svg" alt="a snake eating my contribution graph" />
</picture>

*The snake eats my commits so I don't have to.*

![footer](https://capsule-render.vercel.app/api?type=waving&height=90&color=3C3B6E&section=footer)

</div>
