<h1 align="center">Hey, soy Lucas 👋</h1>

<p align="center">
  <strong>Full Stack Developer · TypeScript · React · Next.js · NestJS</strong>
</p>

<p align="center">
  <a href="https://lsbstack.com"><img src="https://img.shields.io/badge/Portfolio-lsbstack.com-2563EB?style=for-the-badge&logo=vercel&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/lucas-ben%C3%ADtez-b38069291/"><img src="https://img.shields.io/badge/LinkedIn-lucas--benítez-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:lucaspy1943@icloud.com"><img src="https://img.shields.io/badge/Email-lucaspy1943@icloud.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

---

## 🚀 Proyectos en producción

### 🛍️ [Acme Commerce](https://shop.lsbstack.com) — E-commerce Full Stack
[![CI](https://github.com/LucasBenitez7/acme-commerce-starter/actions/workflows/ci.yml/badge.svg)](https://github.com/LucasBenitez7/acme-commerce-starter/actions)

Plataforma e-commerce completa con pagos reales, autenticación avanzada y suite de tests completa.

- **Stripe** (Payment Intents + Webhooks) · pagos reales en producción
- **NextAuth.js v5** — OAuth GitHub, OTP por email, roles usuario/admin
- **Vitest + Playwright E2E** — tests unitarios, integración y E2E con BD aislada
- **CI/CD** con GitHub Actions — lint → tests → E2E en cada push

**Stack:** Next.js 15 · React 19 · TypeScript · Prisma · PostgreSQL · Tailwind CSS · Docker · Vercel

---

### ⚡ [TicketMaster API](https://ticket.lsbstack.com/api/docs) — REST API Alta Concurrencia
[![CI](https://github.com/LucasBenitez7/ticketmaster-api/actions/workflows/ci.yml/badge.svg)](https://github.com/LucasBenitez7/ticketmaster-api/actions)
[![k6 Smoke](https://github.com/LucasBenitez7/ticketmaster-api/actions/workflows/k6-smoke.yml/badge.svg)](https://github.com/LucasBenitez7/ticketmaster-api/actions)

API REST de producción desplegada en AWS EC2 con cero sobreventa garantizada bajo alta concurrencia.

- **Transacciones ACID** — 50 usuarios simultáneos, stock 1 → exactamente 1 checkout ✅
- **BullMQ + Redis** — pagos async con Stripe Webhooks sin bloquear la respuesta
- **Socket.io** — stock actualizado en real-time a todos los clientes
- **k6 load testing** — 500 VUs · p95 < 12ms · 0% errores

**Stack:** NestJS · TypeScript · PostgreSQL · Redis · BullMQ · Socket.io · Stripe · AWS EC2 + S3 · Docker · Cloudflare

---

## 🛠️ Stack

```typescript
const stack = {
  languages:  ["TypeScript", "JavaScript", "SQL"],
  frontend:   ["React 19", "Next.js", "Tailwind CSS", "Zustand", "Zod"],
  backend:    ["NestJS", "Node.js", "Express.js", "REST APIs", "WebSockets"],
  databases:  ["PostgreSQL", "MongoDB", "Firebase", "Prisma ORM", "Redis"],
  testing:    ["Vitest", "Jest", "Playwright", "Testing Library", "MSW", "k6"],
  devops:     ["Docker", "GitHub Actions", "AWS EC2 + S3", "Vercel", "Cloudflare"],
  payments:   ["Stripe (Payment Intents + Webhooks)"],
}
```

---

## 📫 Contacto

Busco posición remota como **Full Stack Developer** o **Backend Developer**.

- 🌐 [lsbstack.com](https://lsbstack.com)
- 💼 [linkedin.com/in/lucas-benítez](https://www.linkedin.com/in/lucas-ben%C3%ADtez-b38069291/)
- 📩 [lucaspy1943@icloud.com](mailto:lucaspy1943@icloud.com)
