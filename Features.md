# 🔐 AccessGrid — Features Overview

AccessGrid is a **modular, extensible authentication & authorization platform** built on top of [SuperTokens](https://supertokens.com).

It transforms SuperTokens from an auth engine into a **complete SaaS-grade identity system**, offering plug-and-play RBAC, multi-tenant onboarding, secure invite flows, and developer-first UX.

---

## ⚙️ Built on SuperTokens Core

AccessGrid leverages the following proven SuperTokens capabilities:

| Category           | SuperTokens Provides                                                    |
|--------------------|-------------------------------------------------------------------------|
| 🔑 Authentication  | Email/password, social login (Google, GitHub), passwordless (OTP/email) |
| 🔄 Sessions        | Secure token rotation, anti-CSRF, theft detection                       |
| 👥 User Management | Signup, login, logout, password reset, email verification               |
| 🧩 Account Linking | Merge social and password identities into one                          |
| 🔐 2FA / MFA       | Support for TOTP, email-based 2FA                                       |
| 🪪 JWT Support     | Secure JWT generation + validation                                      |
| 🧰 SDKs + UI       | Frontend SDKs (React, Next.js), backend SDKs (Node, Go, Python, etc.)   |
| 🛠 Dashboard       | Admin panel to manage users, tenants, and roles                         |
| 🐳 Self-Hosting    | Fully open-source, Docker-compatible deployment                         |

---

## 🚀 What AccessGrid Adds On Top

AccessGrid adds an **opinionated, enterprise-ready DX layer** on top of SuperTokens:

### 🧱 1. Role & Scope-Based Access (RBAC++)

- Roles (`admin`, `user`, `viewer`)
- Scopes (`projects:read`, `users:update`)
- API & UI guards with `withScope()` and `withRole()`

---

### 🏢 2. Multi-Tenant Ready (Team/Org System)

- Create and switch between multiple orgs/teams
- Assign roles scoped per org
- Invite-based team onboarding with expirable links

---

### 🎨 3. Styled UI Component Kit

- Prebuilt Tailwind/Chakra UI components:
  - Login, Signup, 2FA, Reset Password
  - Team switcher, Invite Accept, Permissions modal
- Designed for easy override and theming

---

### 📨 4. Invite System

- Org-linked invite flow via secure email links
- One-time/expirable invites with role binding
- Onboarding screen for first-time users

---

### 🧾 5. Audit Logs

- User-level activity: login, logout, session revoke
- Admin actions: invite sent, role changed, org updated
- Pluggable storage (PostgreSQL / Redis / Custom)

---

### 🛠️ 6. CLI Bootstrapping Tool

- `npx accessgrid init` scaffolds full-stack project with:
  - SuperTokens setup
  - Prisma migrations
  - Sample UI
  - Org + role models
  - API guards

---

### ⚙️ 7. Plugin & Extension System

- Custom plugins to:
  - Log events to Sentry/PostHog
  - Send emails via external provider
  - Add rate limits, metrics, alerts

---

### 🌍 8. Internationalization (i18n)

- Built-in translation support for UI & emails
- Ships with English + i18n scaffold

---

### 💸 (Optional) SaaS Plan Extension

- Stripe integration for paid plans
- Quota enforcement per org
- Plan-based role assignments

---

## 📦 Summary: AccessGrid vs SuperTokens

| Feature Category        | SuperTokens      | AccessGrid Adds                            |
|-------------------------|------------------|---------------------------------------------|
| Auth Flows              | ✅ Core login, session | ✅ UI polish, CLI, DX                         |
| RBAC                    | ✅ Dashboard roles     | ✅ Guarding, scopes, SDK guards               |
| Tenant / Org System     | ✅ Admin UI            | ✅ Invite flow, switcher UI, scoped APIs      |
| Admin Dashboard         | ✅ Basic UI            | ✅ Extended admin UX, team ops                |
| Invite Management       | ❌                  | ✅ Scoped, secure, expirable onboarding       |
| Audit Logs              | ❌                  | ✅ Per-user/org admin tracking                |
| UI Component Kit        | ❌ Minimal flows       | ✅ Full Tailwind/Chakra UI for all flows      |
| Plugin System           | ❌ Override hooks only | ✅ Plugin-ready architecture                  |
| i18n Support            | ❌                  | ✅ Full frontend + email translation          |
| Billing / Plans         | ❌                  | ✅ Optional SaaS extension module             |

---

## 📈 Target Users

- **Developers** building SaaS apps who want full control, self-hosting, and enterprise features
- **Startups** who need fast onboarding, RBAC, and multi-tenant workflows
- **Companies** who want secure identity but don’t want vendor lock-in

---


