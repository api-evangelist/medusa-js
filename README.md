# Medusa (medusa-js)

Medusa is an open-source headless commerce platform written in Node.js and TypeScript, distributed under the MIT license. The Medusa server exposes two REST APIs - a public Store API consumed by storefronts and end-customer clients, and a privileged Admin API consumed by the Medusa Admin dashboard and back-office tooling - both documented with OpenAPI. Around the server the project ships a modular Framework (API Routes, Modules, Module Links, Workflows, Subscribers, Scheduled Jobs, Admin Extensions), the Commerce Modules (cart, payment, customer, pricing, promotion, product, order, inventory, fulfillment, stock location, region, sales channel, tax, currency, API keys, user, auth), the @medusajs/js-sdk TypeScript client, the Medusa CLI (create-medusa-app), the Next.js storefront starter, a remote MCP server that exposes the docs to LLM coding assistants, and Medusa Cloud as an optional managed hosting offering with predictable per-environment pricing and no GMV fees.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Commerce, Headless, eCommerce, Open Source, Node.js, TypeScript, Framework, Modules, Workflows, MCP

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-25

## APIs

### Medusa Store API

Public REST API consumed by storefronts and end-customer clients - carts, products, collections, categories, regions, customers, orders, payments, shipping, returns, gift cards, and store credit. Scoped to one or more sales channels via a publishable API key, with customer-scoped requests authenticated by JWT bearer token or session cookie. Versioned and described with OpenAPI.

**Human URL:** [https://docs.medusajs.com/api/store](https://docs.medusajs.com/api/store)

#### Tags:

 - REST, Storefront, Carts, Orders, Products

#### Properties

- [Documentation](https://docs.medusajs.com/api/store)
- [APIReference](https://docs.medusajs.com/api/store)
- [OpenAPI](https://docs.medusajs.com/api/download/store)
- [OpenAPI](openapi/medusa-js-openapi.yml)
- [Authentication](https://docs.medusajs.com/api/store#authentication)

### Medusa Admin API

Privileged REST API consumed by the Medusa Admin dashboard and back-office tooling - product, inventory, pricing, order, customer, user, and store administration, plus configuration of regions, tax, currencies, payment, and shipping. Authenticated via API tokens, admin sessions, or JWT.

**Human URL:** [https://docs.medusajs.com/api/admin](https://docs.medusajs.com/api/admin)

#### Tags:

 - REST, Admin, Back-Office

#### Properties

- [Documentation](https://docs.medusajs.com/api/admin)
- [APIReference](https://docs.medusajs.com/api/admin)
- [OpenAPI](https://docs.medusajs.com/api/download/admin)
- [Authentication](https://docs.medusajs.com/api/admin#authentication)

### Medusa JS SDK (@medusajs/js-sdk)

Official TypeScript / JavaScript SDK wrapping the Store and Admin REST APIs - typed clients, auth helpers, and ergonomic resource methods. Distributed via npm as @medusajs/js-sdk with shared @medusajs/types.

**Human URL:** [https://docs.medusajs.com/resources/js-sdk](https://docs.medusajs.com/resources/js-sdk)

#### Tags:

 - SDK, JavaScript, TypeScript

#### Properties

- [Documentation](https://docs.medusajs.com/resources/js-sdk)
- [Package](https://www.npmjs.com/package/@medusajs/js-sdk)
- [Repository](https://github.com/medusajs/medusa/tree/develop/packages/core/js-sdk)

### Medusa Framework (Modules, Workflows, Routes)

Server-side framework primitives for extending Medusa - custom API Routes, Modules with their own data models (DML), Module Links, Workflows for transactional business logic, Subscribers and Scheduled Jobs for event-driven and recurring work, and Admin Extensions for the dashboard.

**Human URL:** [https://docs.medusajs.com/learn/fundamentals/framework](https://docs.medusajs.com/learn/fundamentals/framework)

#### Tags:

 - Framework, Workflows, Modules, Extensions

#### Properties

- [Documentation](https://docs.medusajs.com/learn/fundamentals/framework)
- [Repository](https://github.com/medusajs/medusa)

### Medusa Commerce Modules

First-party domain modules that compose into a Medusa application - Cart, Payment, Customer, Pricing, Promotion, Product, Order, Inventory, Fulfillment, Stock Location, Region, Sales Channel, Tax, Currency, API Keys, User, and Auth. Each module ships its own data models, services, and APIs and can be replaced or extended.

**Human URL:** [https://docs.medusajs.com/resources/commerce-modules](https://docs.medusajs.com/resources/commerce-modules)

#### Tags:

 - Modules, Commerce, Domain Models

#### Properties

- [Documentation](https://docs.medusajs.com/resources/commerce-modules)
- [Repository](https://github.com/medusajs/medusa/tree/develop/packages/modules)

### Medusa CLI (create-medusa-app)

Command-line tooling for scaffolding new Medusa projects, generating modules and migrations, running the server in dev, and managing common project tasks.

**Human URL:** [https://docs.medusajs.com/learn/installation](https://docs.medusajs.com/learn/installation)

#### Tags:

 - CLI, Tooling, Developer Experience

#### Properties

- [Documentation](https://docs.medusajs.com/learn/installation)
- [Repository](https://github.com/medusajs/medusa)
- [Package](https://www.npmjs.com/package/create-medusa-app)

### Medusa Next.js Storefront Starter

Reference Next.js storefront talking to the Medusa Store API - cart, checkout, account, product browse, payments, and search. Used as the canonical starting point for headless storefronts.

**Human URL:** [https://docs.medusajs.com/resources/nextjs-starter](https://docs.medusajs.com/resources/nextjs-starter)

#### Tags:

 - Starter, Next.js, Storefront

#### Properties

- [Repository](https://github.com/medusajs/nextjs-starter-medusa)
- [Documentation](https://docs.medusajs.com/resources/nextjs-starter)

### Medusa Docs MCP Server

Remote Model Context Protocol server exposing the Medusa documentation to LLM-powered coding assistants - lets agents look up commerce modules, framework concepts, and APIs while writing Medusa code.

**Human URL:** [https://docs.medusajs.com/learn/introduction/build-with-llms-ai](https://docs.medusajs.com/learn/introduction/build-with-llms-ai)

#### Tags:

 - MCP, AI, LLM, Documentation

#### Properties

- [Documentation](https://docs.medusajs.com/learn/introduction/build-with-llms-ai)

### Medusa Core Repository

Monorepo with the Medusa server, Admin, Commerce Modules, Framework, and packages. MIT-licensed reference for self-hosting and for building modules and plugins.

**Human URL:** [https://github.com/medusajs/medusa](https://github.com/medusajs/medusa)

#### Tags:

 - Open Source, Repository, Monorepo

#### Properties

- [Repository](https://github.com/medusajs/medusa)
- [ReleaseNotes](https://github.com/medusajs/medusa/releases)
- [License](https://github.com/medusajs/medusa/blob/develop/LICENSE)

## Common Properties

- [Website](https://medusajs.com/)
- [Documentation](https://docs.medusajs.com/)
- [APIReference](https://docs.medusajs.com/api/store)
- [APIReference](https://docs.medusajs.com/api/admin)
- [GitHubOrganization](https://github.com/medusajs)
- [GitHubRepository](https://github.com/medusajs/medusa)
- [Pricing](https://medusajs.com/pricing/)
- [Blog](https://medusajs.com/blog/)
- [Support](https://discord.com/invite/medusajs)
- [LLMsTxt](https://docs.medusajs.com/llms.txt)
- [License](https://github.com/medusajs/medusa/blob/develop/LICENSE)
- [LinkedIn](https://www.linkedin.com/company/medusajs/)
- [ReleaseNotes](https://github.com/medusajs/medusa/releases)

## Features

| Name | Description |
|------|-------------|
| Modular Commerce Modules | First-party domain modules (cart, order, product, inventory, pricing, promotion, payment, fulfillment, region, sales channel, tax, currency, auth) that can be swapped or extended. |
| Workflows Engine | Transactional, durable business-logic workflows with compensation steps for orchestrating multi-step commerce operations. |
| Admin Dashboard | Customizable React-based Medusa Admin UI with first-class admin extensions for adding screens, widgets, and routes. |
| Store and Admin REST APIs | Two distinct REST surfaces - public Store API and privileged Admin API - both described with OpenAPI. |
| JS / TypeScript SDK | Typed JS SDK (@medusajs/js-sdk) for both Store and Admin APIs with shared types from @medusajs/types. |
| Next.js Starter | Reference Next.js storefront wired to the Store API as a launchpad for custom storefronts. |
| CLI Tooling | create-medusa-app and the Medusa CLI for scaffolding projects, running dev servers, and managing migrations. |
| Agentic Development (MCP) | Remote MCP server exposing the docs and a Development Agent that lets LLM coding assistants build on Medusa. |
| Medusa Cloud | Optional managed hosting with GitHub-based deploys, autoscaling, and no GMV-based fees. |
| MIT License | Permissive open-source license with no vendor lock-in and the ability to self-host the full stack. |

## Use Cases

| Name | Description |
|------|-------------|
| Headless DTC Storefronts | Power Next.js / React Native / native storefronts for direct-to-consumer brands using the Store API and JS SDK. |
| B2B Commerce | Build company-account, quoting, and approval flows on top of the Commerce Modules and Workflows engine. |
| Marketplaces | Use sales channels, regions, and stock locations to model multi-vendor and multi-store marketplaces. |
| Composable Commerce Replatforming | Replace Shopify, BigCommerce, or Magento with a fully owned, self-hostable commerce backend. |
| AI-Native Commerce | Drive merchandising, support, and operations from LLM agents using the MCP server and admin tooling. |
| Custom Checkout Experiences | Implement bespoke checkout, payment, and pricing flows by composing modules and workflows. |
| Quick Commerce & Logistics | Model stock locations, fulfillment, and regions for last-mile and on-demand delivery models. |
| Internal Commerce Platforms | Stand up an internal commerce backbone for catalog, orders, and fulfillment shared across brands or business units. |

## Integrations

| Name | Description |
|------|-------------|
| Next.js | Official Next.js storefront starter (nextjs-starter-medusa) wired to the Store API. |
| Stripe | Payment provider integration for card payments and saved methods via the Payment module. |
| PayPal | PayPal payment provider integration via the Payment module. |
| Algolia / MeiliSearch / Typesense | Search integrations for product catalog indexing and storefront search. |
| SendGrid / Resend | Notification providers for transactional email through the Notification module. |
| AWS S3 / MinIO | File storage providers for product images and assets. |
| PostgreSQL | Primary supported database engine for the Medusa server. |
| Redis | Used for caching, event bus, and queues in production deployments. |
| Model Context Protocol (MCP) | Remote MCP server exposes the Medusa docs to Claude, Cursor, and other MCP-aware coding assistants. |
| GitHub | GitHub-based deployments and source-of-truth for Medusa Cloud environments. |

## Solutions

| Name | Description |
|------|-------------|
| Medusa Core (Self-Hosted) | Free, MIT-licensed open-source server, Admin, framework, and commerce modules deployable to any Node.js host. |
| Medusa Cloud - Develop | Entry managed tier with GitHub deploys, dev agent, and a shared server starting at $29/mo. |
| Medusa Cloud - Launch | Production-ready managed tier with autoscaling, custom domains, automatic backups, and zero-downtime deploys at $99/mo. |
| Medusa Cloud - Scale | Growth tier with background workers, priority support, and higher edge request quotas at $299/mo. |
| Medusa Cloud - Enterprise | SLA-backed enterprise tier with core-team access, custom agentic workflows, and implementation support. |
| Medusa Experts | Curated partner network of agencies and consultancies delivering Medusa implementations. |

## Artifacts

Machine-readable API specifications and supporting commercial / operational descriptors.

### OpenAPI

- [Medusa Store API (best-effort)](openapi/medusa-js-openapi.yml)

### Plans

- [Medusa Plans & Pricing](plans/medusa-js-plans-pricing.yml)

### Rate Limits

- [Medusa Rate Limits](rate-limits/medusa-js-rate-limits.yml)

### FinOps

- [Medusa FinOps Alignment](finops/medusa-js-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
