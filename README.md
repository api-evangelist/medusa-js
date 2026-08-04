# Medusa (medusa-js)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Medusa is an open-source headless commerce platform written in Node.js and TypeScript, distributed under the MIT license. The Medusa server exposes two REST APIs - a public Store API consumed by storefronts and end-customer clients, and a privileged Admin API consumed by the Medusa Admin dashboard and back-office tooling - both documented with OpenAPI. Around the server the project ships a modular Framework (API Routes, Modules, Module Links, Workflows, Subscribers, Scheduled Jobs, Admin Extensions), the Commerce Modules (cart, payment, customer, pricing, promotion, product, order, inventory, fulfillment, stock location, region, sales channel, tax, currency, API keys, user, auth), the @medusajs/js-sdk TypeScript client, the Medusa CLI (create-medusa-app), the Next.js storefront starter, a remote MCP server that exposes the docs to LLM coding assistants, and Medusa Cloud as an optional managed hosting offering with predictable per-environment pricing and no GMV fees.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/medusa-js/refs/heads/main/apis.yml)

## Tags

- Commerce
- Headless
- eCommerce
- Open Source
- Node.js
- TypeScript
- Framework
- Modules
- Workflows
- MCP

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-25

## APIs

### Medusa Store API

Public REST API consumed by storefronts and end-customer clients - carts, products, collections, categories, regions, customers, orders, payments, shipping, returns, gift cards, and store credit. Scoped to one or more sales channels via a publishable API key, with customer-scoped requests authenticated by JWT bearer token or session cookie. Versioned and described with OpenAPI.

- **Human URL:** [https://docs.medusajs.com/api/store](https://docs.medusajs.com/api/store)
- **Base URL:** `https://docs.medusajs.com/api/store`

#### Tags

- REST
- Storefront
- Carts
- Orders
- Products

#### Properties

- [Documentation](https://docs.medusajs.com/api/store)
- [API Reference](https://docs.medusajs.com/api/store)
- [OpenAPI](https://docs.medusajs.com/api/download/store) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/medusa-js-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Authentication](https://docs.medusajs.com/api/store#authentication)

### Medusa Admin API

Privileged REST API consumed by the Medusa Admin dashboard and back-office tooling - product, inventory, pricing, order, customer, user, and store administration, plus configuration of regions, tax, currencies, payment, and shipping. Authenticated via API tokens, admin sessions, or JWT.

- **Human URL:** [https://docs.medusajs.com/api/admin](https://docs.medusajs.com/api/admin)
- **Base URL:** `https://docs.medusajs.com/api/admin`

#### Tags

- REST
- Admin
- Back-Office

#### Properties

- [Documentation](https://docs.medusajs.com/api/admin)
- [API Reference](https://docs.medusajs.com/api/admin)
- [OpenAPI](https://docs.medusajs.com/api/download/admin) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Authentication](https://docs.medusajs.com/api/admin#authentication)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Medusa JS SDK (@medusajs/js-sdk)

Official TypeScript / JavaScript SDK wrapping the Store and Admin REST APIs - typed clients, auth helpers, and ergonomic resource methods. Distributed via npm as @medusajs/js-sdk with shared @medusajs/types.

- **Human URL:** [https://docs.medusajs.com/resources/js-sdk](https://docs.medusajs.com/resources/js-sdk)
- **Base URL:** `https://www.npmjs.com/package/@medusajs/js-sdk`

#### Tags

- SDK
- JavaScript
- TypeScript

#### Properties

- [Documentation](https://docs.medusajs.com/resources/js-sdk)
- [Package](https://www.npmjs.com/package/@medusajs/js-sdk)
- [Repository](https://github.com/medusajs/medusa/tree/develop/packages/core/js-sdk)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Medusa Framework (Modules, Workflows, Routes)

Server-side framework primitives for extending Medusa - custom API Routes, Modules with their own data models (DML), Module Links, Workflows for transactional business logic, Subscribers and Scheduled Jobs for event-driven and recurring work, and Admin Extensions for the dashboard.

- **Human URL:** [https://docs.medusajs.com/learn/fundamentals/framework](https://docs.medusajs.com/learn/fundamentals/framework)
- **Base URL:** `https://docs.medusajs.com/learn/fundamentals/framework`

#### Tags

- Framework
- Workflows
- Modules
- Extensions

#### Properties

- [Documentation](https://docs.medusajs.com/learn/fundamentals/framework)
- [Repository](https://github.com/medusajs/medusa)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Medusa Commerce Modules

First-party domain modules that compose into a Medusa application - Cart, Payment, Customer, Pricing, Promotion, Product, Order, Inventory, Fulfillment, Stock Location, Region, Sales Channel, Tax, Currency, API Keys, User, and Auth. Each module ships its own data models, services, and APIs and can be replaced or extended.

- **Human URL:** [https://docs.medusajs.com/resources/commerce-modules](https://docs.medusajs.com/resources/commerce-modules)
- **Base URL:** `https://docs.medusajs.com/resources/commerce-modules`

#### Tags

- Modules
- Commerce
- Domain Models

#### Properties

- [Documentation](https://docs.medusajs.com/resources/commerce-modules)
- [Repository](https://github.com/medusajs/medusa/tree/develop/packages/modules)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Medusa CLI (create-medusa-app)

Command-line tooling for scaffolding new Medusa projects, generating modules and migrations, running the server in dev, and managing common project tasks.

- **Human URL:** [https://docs.medusajs.com/learn/installation](https://docs.medusajs.com/learn/installation)
- **Base URL:** `https://github.com/medusajs/medusa`

#### Tags

- CLI
- Tooling
- Developer Experience

#### Properties

- [Documentation](https://docs.medusajs.com/learn/installation)
- [Repository](https://github.com/medusajs/medusa)
- [Package](https://www.npmjs.com/package/create-medusa-app)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Medusa Next.js Storefront Starter

Reference Next.js storefront talking to the Medusa Store API - cart, checkout, account, product browse, payments, and search. Used as the canonical starting point for headless storefronts.

- **Human URL:** [https://docs.medusajs.com/resources/nextjs-starter](https://docs.medusajs.com/resources/nextjs-starter)
- **Base URL:** `https://github.com/medusajs/nextjs-starter-medusa`

#### Tags

- Starter
- Next.js
- Storefront

#### Properties

- [Repository](https://github.com/medusajs/nextjs-starter-medusa)
- [Documentation](https://docs.medusajs.com/resources/nextjs-starter)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Medusa Docs MCP Server

Remote Model Context Protocol server exposing the Medusa documentation to LLM-powered coding assistants - lets agents look up commerce modules, framework concepts, and APIs while writing Medusa code.

- **Human URL:** [https://docs.medusajs.com/learn/introduction/build-with-llms-ai](https://docs.medusajs.com/learn/introduction/build-with-llms-ai)
- **Base URL:** `https://docs.medusajs.com/learn/introduction/build-with-llms-ai`

#### Tags

- MCP
- AI
- LLM
- Documentation

#### Properties

- [Documentation](https://docs.medusajs.com/learn/introduction/build-with-llms-ai)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Medusa Core Repository

Monorepo with the Medusa server, Admin, Commerce Modules, Framework, and packages. MIT-licensed reference for self-hosting and for building modules and plugins.

- **Human URL:** [https://github.com/medusajs/medusa](https://github.com/medusajs/medusa)
- **Base URL:** `https://github.com/medusajs/medusa`

#### Tags

- Open Source
- Repository
- Monorepo

#### Properties

- [Repository](https://github.com/medusajs/medusa)
- [Release Notes](https://github.com/medusajs/medusa/releases)
- [License](https://github.com/medusajs/medusa/blob/develop/LICENSE)
- [Postman Collection](collections/medusa-js.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/medusa-js.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://medusajs.com/)
- [Documentation](https://docs.medusajs.com/)
- [API Reference](https://docs.medusajs.com/api/store)
- [API Reference](https://docs.medusajs.com/api/admin)
- [GitHub Organization](https://github.com/medusajs)
- [GitHub Repository](https://github.com/medusajs/medusa)
- [Pricing](https://medusajs.com/pricing/)
- [Blog](https://medusajs.com/blog/)
- [Support](https://discord.com/invite/medusajs)
- [L L Ms Txt](https://docs.medusajs.com/llms.txt)
- [License](https://github.com/medusajs/medusa/blob/develop/LICENSE)
- [LinkedIn](https://www.linkedin.com/company/medusajs/)
- [Release Notes](https://github.com/medusajs/medusa/releases)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
