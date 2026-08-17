# FORGE

### AI-Powered Startup Creation & Venture Operating Platform

**Developed during a 3-month internship at Algo Force AI.**

🌐 **Live Demo:** [https://forge26.netlify.app/](https://forge26.netlify.app/)

[![Open FORGE](https://img.shields.io/badge/🚀%20Open%20FORGE-Live%20Demo-7C3AED?style=for-the-badge)](https://forge26.netlify.app/)

---

## 📌 Project Information

| | |
|---|---|
| **Project** | FORGE |
| **Organization** | Algo Force AI |
| **Engagement** | 3-Month Internship |
| **Role** | Full-Stack / AI Engineering |
| **Project Type** | AI-Powered SaaS Platform |
| **Focus** | AI, Full-Stack Development, Startup Intelligence |
| **Deployment** | Cloud / Web Application |

> This repository is a public project showcase. Certain implementation details, credentials, datasets, infrastructure configuration, proprietary business logic, and organization-specific information are intentionally excluded due to confidentiality requirements.

---

## 🚀 Project Overview

FORGE brings the major startup-building workflows into a single, unified platform, connecting founders, builders, and investors across the full venture lifecycle:

**Idea → Validation → Team Building → Startup Creation → Funding → Growth → Scale**

The platform provides role-specific workspaces for:

- 👨‍🚀 **Founders**
- 👨‍💻 **Builders**
- 💰 **Investors**

---

## 👥 Platform / Target Users

### Founders
- Create and validate ideas
- Build startup teams
- Recruit builders
- Create projects
- Explore funding opportunities
- Manage startup workflows

### Builders
- Discover startup projects
- Explore opportunities
- Apply to projects
- Manage skills and profiles
- Collaborate with startup teams
- Track assigned work

### Investors
- Discover startups
- Evaluate opportunities
- Access startup intelligence
- Shortlist opportunities
- Track investment workflows

---

## 🧩 Core Platform Capabilities

- 💡 **Idea Exchange** — Idea discovery, validation, voting, and AI-assisted refinement
- 🤝 **Founder & Builder Matching** — Profiles, project discovery, applications, and collaboration
- 🚀 **Startup Creation** — Startup formation, team building, projects, and execution workflows
- 🛠️ **Builder Marketplace** — Startup opportunities, skill-based matching, and project collaboration
- 💰 **Investor Workflows** — Startup discovery, evaluation, shortlisting, and funding workflows
- 🧠 **Startup Intelligence** — AI-assisted market, risk, competitor, and startup-readiness analysis

---

## 🤖 AI Intelligence Layer

FORGE uses AI to support workflows such as:

- Idea validation
- Market analysis
- Competitor analysis
- Business model evaluation
- Experiment generation
- Pitch improvement
- Investor readiness
- Roadmap generation
- Startup scoring

### AI Provider Architecture

The application uses a provider abstraction layer so AI workflows are not tightly coupled to a single provider.

```text
              AI Request
                  │
                  ▼
           Provider Router
                  │
          ┌───────┴───────┐
          ▼               ▼
       Primary          Fallback
       Provider         Provider
          │               │
          └───────┬───────┘
                  ▼
             AI Response
```

*API keys, private endpoints, internal prompts, and provider configuration values are intentionally not disclosed.*

---

## 🏗️ High-Level System Architecture

```text
                         FORGE PLATFORM
                              │
                              ▼
                    ┌──────────────────┐
                    │   Next.js Web    │
                    │ React / TypeScript│
                    └────────┬─────────┘
                             │
                ┌────────────┴────────────┐
                ▼                         ▼
       ┌─────────────────┐       ┌─────────────────┐
       │    Supabase     │       │  FastAPI AI     │
       │                 │       │    Service      │
       │ Authentication  │       │                 │
       │ PostgreSQL      │       │ LangGraph       │
       │ Realtime        │       │ AI Workflows    │
       │ RLS             │       │ Provider Layer  │
       └─────────────────┘       └────────┬────────┘
                                          │
                                          ▼
                                  ┌───────────────┐
                                  │ AI Providers  │
                                  │ Primary +     │
                                  │ Fallback      │
                                  └───────────────┘

                 Infrastructure & Observability
                       Docker · Prometheus · Grafana
```

This diagram is intentionally high-level. Internal service URLs, network topology, database hostnames, project IDs, and connection strings are not included.

---

## 🛠️ Technology Stack

**Frontend**
- Next.js
- React
- TypeScript
- Tailwind CSS

**Backend**
- FastAPI
- Python
- REST APIs

**Database & Authentication**
- Supabase
- PostgreSQL
- Supabase Authentication
- Row Level Security
- Supabase Realtime
- OAuth

**AI**
- LangGraph
- Google Gemini
- Groq
- AI Provider Abstraction (Primary / Fallback Architecture)

**Infrastructure**
- Docker
- Docker Compose
- Cloud Deployment

**Observability**
- Prometheus
- Grafana

**Development**
- Git
- GitHub
- npm
- Python

---

## 🔑 Authentication & Data

FORGE uses Supabase for authentication and data persistence, including OAuth-based sign-in, session management, and role-based access control. PostgreSQL (via Supabase) backs the application's persistent data, with Row Level Security enforcing access boundaries and Supabase Realtime powering live updates across role-based workspaces.

*Schema details, table structures, and connection configuration are not published in this repository.*

---

## 👨‍💻 My Contribution

### 3-Month Internship at Algo Force AI

FORGE was a collaborative, organization-built platform. During my internship, I contributed to the project across the following areas:

- **Frontend Engineering** — Built and refined Next.js/TypeScript interfaces, dashboards, onboarding flows, and responsive role-based experiences
- **Backend Engineering** — Worked with FastAPI services and API workflows, and contributed to backend integration
- **Database Engineering** — Integrated Supabase/PostgreSQL for persistent application data, authentication, and realtime workflows
- **Authentication & Authorization** — Worked on authentication flows, OAuth, sessions, protected routes, and role-based access
- **AI Engineering** — Worked with LangGraph-based AI workflows and contributed to the AI provider abstraction/fallback mechanism supporting startup intelligence features
- **Infrastructure** — Worked with Docker-based development and cloud deployment configuration
- **Observability** — Integrated and used Prometheus and Grafana for application monitoring and visualization
- **Testing & Debugging** — Worked on authentication persistence, database integration, role routing, responsive behavior, realtime functionality, and deployment issue investigation

```text
Frontend
   │
Backend
   │
Database
   │
Authentication
   │
AI
   │
Infrastructure
   │
Observability
   │
Deployment
```

*This section reflects my individual contribution within a larger, organization-owned project — not sole authorship of the platform.*

---

## 📈 Engineering Highlights

- Role-based SaaS architecture
- Persistent cloud database
- Authentication and OAuth
- Realtime application workflows
- AI-assisted startup intelligence
- AI provider abstraction and fallback
- Modular frontend architecture
- API-driven backend services
- Containerized development
- Application observability
- Cloud deployment
- Responsive web experience

---

## 🌐 Live Project

[![Open FORGE](https://img.shields.io/badge/🚀%20Open%20FORGE-Live%20Demo-7C3AED?style=for-the-badge)](https://forge26.netlify.app/)

🌐 **Live Application:** [https://forge26.netlify.app/](https://forge26.netlify.app/)

---

## 🔐 Security & Confidentiality

This repository is intended as a **public portfolio and project showcase**, not internal engineering documentation. It intentionally excludes:

- API keys and secrets
- Service-role credentials
- Database credentials and connection strings
- Private environment variable values
- Proprietary datasets
- Internal prompts
- Private API endpoints
- Organization-specific infrastructure details
- Confidential business logic
- Internal monitoring configuration and URLs

Environment variables must be supplied through local or deployment configuration and are never committed to version control.

---

## 📚 Project Context

FORGE was developed as part of a **3-month internship at Algo Force AI**, providing hands-on experience building and integrating a multi-layer AI-powered SaaS platform — spanning frontend engineering, backend services, databases, authentication, AI workflows, infrastructure, observability, and deployment.

---

## 📋 Project Status

This repository is a curated public showcase of a real, internally-deployed platform. It is maintained as a portfolio reference and is not the organization's production codebase.
