# Hey, soy Lucas 👋

**Full Stack Developer · TypeScript · JavaScript · Python**

[![Portfolio](https://img.shields.io/badge/Portfolio-lsbstack.com-2563EB?style=for-the-badge&logo=vercel&logoColor=white)](https://lsbstack.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-lucas--benítez-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucas-ben%C3%ADtez-b38069291/)
[![Email](https://img.shields.io/badge/Email-lucaspy1943@icloud.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:lucaspy1943@icloud.com)

---

## 🚀 Proyectos en producción

### 🏦 [RiskCore](https://github.com/LucasBenitez7/risk-core) — Microservicios & Event-Driven Architecture

[![CI Policy](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-policy-service.yml/badge.svg)](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-policy-service.yml)
[![CI Claims](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-claims-service.yml/badge.svg)](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-claims-service.yml)
[![CI Audit](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-audit-service.yml/badge.svg)](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-audit-service.yml)
[![CI Notification](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-notification-service.yml/badge.svg)](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-notification-service.yml)
[![CI Frontend](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-frontend.yml/badge.svg)](https://github.com/LucasBenitez7/risk-core/actions/workflows/ci-frontend.yml)

Sistema backend de microservicios que simula el core de una aseguradora enterprise — gestión de pólizas, siniestros, notificaciones y auditoría inmutable con event-driven architecture.

- **4 microservicios Django** con Database per Service, comunicación async via Kafka (6 topics)
- **Circuit Breaker** (pybreaker) + **Outbox Pattern** para resiliencia y garantía de entrega de eventos
- **Gateway Nginx** con validación JWT centralizada, rate limiting y X-Request-ID para trazabilidad completa
- **Dashboard Next.js 15** (App Router + RSC) con feed de eventos en tiempo real via WebSockets
- **Observabilidad completa**: structlog → Loki, Prometheus, 5 dashboards Grafana + alertas automáticas

**Stack:** Django 5.2 · DRF · Apache Kafka · Next.js 15 · TypeScript · PostgreSQL · Redis · Celery · Nginx · Locust · Grafana · Prometheus · Loki · Docker

---

### 🛍️ [LSB Shop](https://shop.lsbstack.com) — E-commerce Full Stack · Next.js 15 + Django

[![CI Backend](https://github.com/LucasBenitez7/lsb-shop/actions/workflows/ci.yml/badge.svg)](https://github.com/LucasBenitez7/lsb-shop/actions)
[![CI Frontend](https://github.com/LucasBenitez7/lsb-shop/actions/workflows/ci-frontend.yml/badge.svg)](https://github.com/LucasBenitez7/lsb-shop/actions)

Tienda de ropa online completa con arquitectura full stack desacoplada: frontend Next.js 15 (pura UI) + API Django 5.2/DRF con patrón services/selectors. Pagos reales con Stripe, autenticación con Google OAuth, carrito persistente en Redis y suite de tests con cobertura ≥80% enforced en CI.

- **Arquitectura desacoplada**: Next.js (Vercel) + Django/DRF (Railway), deploy y escalado independientes. API documentada con OpenAPI/Swagger autogenerado
- **Autenticación completa**: JWT en cookies httpOnly, Google OAuth (django-allauth), roles admin/user/demo, refresh transparente en el cliente
- **Carrito en Redis** con TTL 7 días, fusión automática guest → usuario al login, sin hits a PostgreSQL en lecturas
- **Tareas async con Celery**: emails transaccionales via Resend (confirmación de pedido, verificación, reset), limpieza de carritos, cleanup de imágenes huérfanas en Cloudinary

**Stack:** Next.js 15 · React 19 · TypeScript · Tailwind CSS v4 · Radix UI · Zustand · Django 5.2 · DRF · Python 3.13 · PostgreSQL · Redis · Celery · Stripe · Cloudinary · JWT · Google OAuth · Docker · Railway · Vercel · GitHub Actions · Vitest · Playwright · pytest

---

### ⚡ [TicketMaster API](https://ticket.lsbstack.com/api/docs) — REST API Alta Concurrencia

[![CI](https://github.com/LucasBenitez7/ticketmaster-api/actions/workflows/ci.yml/badge.svg)](https://github.com/LucasBenitez7/ticketmaster-api/actions)
[![k6 Smoke](https://github.com/LucasBenitez7/ticketmaster-api/actions/workflows/k6-smoke.yml/badge.svg)](https://github.com/LucasBenitez7/ticketmaster-api/actions)

API REST de alto rendimiento con cero sobreventa bajo carga, transacciones ACID verificadas con k6, pagos async con BullMQ y WebSockets en tiempo real.

- 500 VUs · p95 < 12ms · 0% errores
- 50 usuarios simultáneos · stock 1 → exactamente 1 checkout ✅

**Stack:** NestJS · TypeScript · PostgreSQL · Redis · BullMQ · Socket.io · Stripe · AWS EC2 + S3 · Docker · Cloudflare

---

### 🐍 [BookingAPI](https://booking.lsbstack.com/docs) — REST API Python · Arquitectura Hexagonal

[![CI](https://github.com/LucasBenitez7/booking-api/actions/workflows/ci.yml/badge.svg)](https://github.com/LucasBenitez7/booking-api/actions)

API REST de gestión de reservas con arquitectura hexagonal — dominio en Python puro sin dependencias externas, infraestructura completamente intercambiable. Workers Celery, caché Redis e infraestructura Kubernetes lista para producción.

**Stack:** Python 3.12 · FastAPI · SQLAlchemy 2 · PostgreSQL · Alembic · Celery · Redis · Docker · Kubernetes · Railway · GitHub Actions

---

## 🛠️ Stack


```
const stack = {
  languages:      ["TypeScript", "JavaScript", "Python"],
  frontend:       ["React 19", "Next.js 15", "Tailwind CSS v4", "Radix UI",
                   "Zustand", "Zod", "React Hook Form", "Framer Motion"],
  backend_node:   ["NestJS", "Express.js", "Prisma ORM", "BullMQ", "WebSockets", "Socket.io"],
  backend_python: ["Django 5.2", "Django REST Framework", "Django Channels",
                   "FastAPI", "confluent-kafka", "Celery", "SQLAlchemy 2",
                   "Alembic", "Pydantic v2", "structlog", "pybreaker", "uv", "Ruff"],
  databases:      ["PostgreSQL", "Redis", "MongoDB", "Firebase", "Neon"],
  testing:        ["Vitest", "Playwright", "Testing Library", "pytest",
                   "factory-boy", "Locust", "k6", "Newman", "mypy", "MSW"],
  devops:         ["Git", "GitHub Actions", "Docker", "Nginx",
                   "Grafana", "Prometheus", "Loki", "AWS EC2 + S3",
                   "Railway", "Vercel", "Cloudflare"],
  metodologias:   ["SDLC", "GitFlow", "ADRs", "Conventional Commits",
                   "Event-Driven Architecture", "Circuit Breaker", "Outbox Pattern",
                   "Services/Selectors Pattern"],
}
```


---

## 📫 Contacto

Busco posición como **Full Stack Developer** o **Backend Developer**.

- 🌐 [lsbstack.com](https://lsbstack.com)
- 💼 [linkedin.com/in/lucas-benítez](https://www.linkedin.com/in/lucas-ben%C3%ADtez-b38069291/)
- 📩 [lucaspy1943@icloud.com](mailto:lucaspy1943@icloud.com)
