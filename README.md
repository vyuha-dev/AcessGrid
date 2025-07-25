# AcessGrid
AccessGrid is a modular, extensible authentication &amp; authorization platform built on top of SuperTokens (https://supertokens.com).


accessgrid/
├── prisma/
│   ├── schema.prisma
│   └── seed.js
│
├── src/
│   ├── config/
│   │   ├── index.js
│   │   ├── supertokens.js
│   │   ├── logger.js
│   │   └── redis.js
│   │
│   ├── middleware/
│   │   ├── auth.js
│   │   ├── errorHandler.js
│   │   └── rateLimiter.js
│   │
│   ├── modules/
│   │   ├── auth/
│   │   │   ├── auth.routes.js
│   │   │   ├── auth.controller.js
│   │   │   ├── auth.service.js
│   │   │   └── index.js
│   │   │
│   │   ├── user/
│   │   │   ├── user.model.js
│   │   │   ├── user.controller.js
│   │   │   ├── user.service.js
│   │   │   └── index.js
│   │   │
│   │   ├── roles/
│   │   │   └── roles.service.js
│   │   │
│   │   └── tenant/
│   │       └── tenant.service.js
│   │
│   ├── routes/
│   │   └── index.js          # Combines all module routes
│   │
│   ├── utils/
│   │   ├── auditLog.js
│   │   ├── response.js
│   │   └── validator.js
│   │
│   └── server.js
│
├── .env
├── .env.example
├── .gitignore
├── package.json
└── README.md
