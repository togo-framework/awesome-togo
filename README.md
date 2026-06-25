<div align="center">
  <img src="https://to-go.dev/togo-mark.svg" alt="togo" height="96" />
  <h1>Awesome togo <a href="https://github.com/sindresorhus/awesome"><img src="https://awesome.re/badge.svg" alt="Awesome"/></a></h1>
  <p><strong>A curated directory of everything in the <a href="https://to-go.dev">togo</a> ecosystem</strong> — the open-source, API-first full-stack Go&nbsp;+&nbsp;React framework with a Laravel-artisan-grade CLI.</p>
  <p>
    <a href="https://to-go.dev/marketplace"><img src="https://img.shields.io/badge/marketplace-to--go.dev-1FC7DC" /></a>
    <img src="https://img.shields.io/badge/plugins-120+-2C7BE2" />
    <a href="https://www.npmjs.com/package/@togo-framework/cli"><img src="https://img.shields.io/npm/v/@togo-framework/cli?label=cli" /></a>
    <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue" /></a>
  </p>
</div>

> Browse, search and install everything at **[to-go.dev/marketplace](https://to-go.dev/marketplace)**. Install any plugin with `togo install togo-framework/<name>`.

## Contents

- [Core](#core)
- [Authentication](#authentication)
- [Database & ORM](#database--orm)
- [Cache](#cache)
- [Storage](#storage)
- [Search](#search)
- [Mail](#mail)
- [Notifications](#notifications)
- [Realtime](#realtime)
- [Queue, Workers & Workflow](#queue-workers--workflow)
- [Logging](#logging)
- [AI Kit](#ai-kit)
- [Payments & Billing](#payments--billing)
- [Deploy](#deploy)
- [DNS, Proxy & Gateway](#dns-proxy--gateway)
- [Tunnels](#tunnels)
- [Chat Bots](#chat-bots)
- [i18n, Location & Settings](#i18n-location--settings)
- [Multi-tenancy (SaaS)](#multi-tenancy-saas)
- [Documents](#documents)
- [Contacts & CRM](#contacts--crm)
- [Dev & Testing](#dev--testing)
- [Supabase](#supabase)
- [SEO](#seo)
- [Contributing](#contributing)

## Core

The framework, CLI, templates and first-party apps.

- [`togo`](https://github.com/togo-framework/togo) — Go, the artisan way — microkernel of the togo framework (Go + sqlc + Atlas + GraphQL/OpenAPI + Next.js)
- [`cli`](https://github.com/togo-framework/cli) — The togo CLI — Laravel-artisan-like generators, codegen, plugins, MCP, deploy
- [`create-togo-app`](https://github.com/togo-framework/create-togo-app) — Project template for togo, rendered by `togo new`
- [`dashboard`](https://github.com/togo-framework/dashboard) — togo dashboard + auth UI (depends on auth)
- [`mcp`](https://github.com/togo-framework/mcp) — MCP server exposing togo generators to AI agents (Claude Code, Cursor, …)
- [`mcp-web`](https://github.com/togo-framework/mcp-web) — Public MCP server for togo — docs, plugins, and plugin submission for agents (mcp.to-go.dev).
- [`plugin-template`](https://github.com/togo-framework/plugin-template) — Starter template for togo plugins
- [`claude-togo`](https://github.com/togo-framework/claude-togo) — Official ToGO plugin for Claude Code — scaffold & drive togo apps with AI (commands, agents, hooks + auto-connected MCP).
- [`to-go.dev`](https://github.com/togo-framework/to-go.dev) — to-go.dev — the togo framework website: landing, docs, install.sh/update.sh.
- [`ui`](https://github.com/togo-framework/ui) — togo UI kit — prism-style admin + auth components (Storybook). RTL-ready, dark-first.

## Authentication

- **[`auth`](https://github.com/togo-framework/auth) — togo base auth: JWT + RBAC + multi-guard, Supabase/GoTrue first-class, OAuth/Firebase/WorkOS as plugins**
- [`auth-dev`](https://github.com/togo-framework/auth-dev) — Developer login for togo auth (dev-only)
- [`auth-firebase`](https://github.com/togo-framework/auth-firebase) — Firebase Authentication driver for togo auth
- [`auth-oauth`](https://github.com/togo-framework/auth-oauth) — OAuth2 social login for togo auth
- [`auth-session-redis`](https://github.com/togo-framework/auth-session-redis) — Redis session store for togo auth
- [`auth-workos`](https://github.com/togo-framework/auth-workos) — WorkOS SSO/SAML driver for togo auth

## Database & ORM

- **[`db`](https://github.com/togo-framework/db) — togo database stack — the togo-postgres image (ParadeDB: pg_search + pgvector + pg_analytics, plus pg_cron + pg_partman) and the batteries-included compose.**
- **[`orm`](https://github.com/togo-framework/orm) — togo ORM: driver-agnostic query builder (SQLi-validated)**
- [`db-mongodb`](https://github.com/togo-framework/db-mongodb)
- [`db-mysql`](https://github.com/togo-framework/db-mysql)
- [`db-postgres`](https://github.com/togo-framework/db-postgres)
- [`db-supabase`](https://github.com/togo-framework/db-supabase) — Postgres/Supabase driver for togo ORM

## Cache

- **[`cache`](https://github.com/togo-framework/cache) — togo cache provider plugin**
- [`cache-redis`](https://github.com/togo-framework/cache-redis) — Redis driver for togo cache

## Storage

- **[`storage`](https://github.com/togo-framework/storage) — togo storage provider plugin**
- [`storage-gdrive`](https://github.com/togo-framework/storage-gdrive) — togo storage driver
- [`storage-r2`](https://github.com/togo-framework/storage-r2) — togo storage driver
- [`storage-s3`](https://github.com/togo-framework/storage-s3) — togo storage driver
- [`storage-supabase`](https://github.com/togo-framework/storage-supabase) — Supabase Storage driver for togo

## Search

- **[`search`](https://github.com/togo-framework/search) — togo search: ParadeDB default + ES/OpenSearch plugins**
- [`search-algolia`](https://github.com/togo-framework/search-algolia) — Algolia driver for togo full-text search
- [`search-elasticsearch`](https://github.com/togo-framework/search-elasticsearch) — Elasticsearch/OpenSearch driver for togo search
- [`search-meilisearch`](https://github.com/togo-framework/search-meilisearch) — Meilisearch driver for togo full-text search
- [`search-typesense`](https://github.com/togo-framework/search-typesense) — Typesense driver for togo full-text search

## Mail

- **[`mail`](https://github.com/togo-framework/mail) — togo mail: SMTP + driver plugins (SES/Resend)**
- [`mail-resend`](https://github.com/togo-framework/mail-resend) — Resend driver for togo mail
- [`mail-sendgrid`](https://github.com/togo-framework/mail-sendgrid) — SendGrid driver for togo mail

## Notifications

- **[`notifications`](https://github.com/togo-framework/notifications) — togo notifications: channels (mail/broadcast/db) + push plugins**
- [`notifications-discord`](https://github.com/togo-framework/notifications-discord) — togo notifications-discord notifications channel
- [`notifications-fcm`](https://github.com/togo-framework/notifications-fcm) — Firebase Cloud Messaging (HTTP v1) push channel for togo notifications
- [`notifications-onesignal`](https://github.com/togo-framework/notifications-onesignal) — OneSignal push channel for togo notifications
- [`notifications-pusher`](https://github.com/togo-framework/notifications-pusher) — Pusher Channels broadcast channel for togo notifications
- [`notifications-slack`](https://github.com/togo-framework/notifications-slack) — togo notifications-slack notifications channel
- [`notifications-webpush`](https://github.com/togo-framework/notifications-webpush) — togo notifications-webpush notifications channel

## Realtime

- **[`realtime`](https://github.com/togo-framework/realtime) — togo realtime provider plugin**
- [`realtime-grpc`](https://github.com/togo-framework/realtime-grpc) — togo plugin: realtime-grpc
- [`realtime-nats`](https://github.com/togo-framework/realtime-nats) — togo plugin: realtime-nats
- [`realtime-ws`](https://github.com/togo-framework/realtime-ws) — WebSocket realtime transport for togo

## Queue, Workers & Workflow

- **[`queue`](https://github.com/togo-framework/queue) — togo queue provider plugin**
- **[`worker`](https://github.com/togo-framework/worker) — togo worker: supervised multi-threaded worker pools**
- **[`workflow`](https://github.com/togo-framework/workflow) — togo workflow plugin**

## Logging

- **[`log`](https://github.com/togo-framework/log) — togo logging: levels, text/json, file output**
- [`log-datadog`](https://github.com/togo-framework/log-datadog) — Datadog log shipping for togo — forwards slog logs to Datadog Logs (HTTP intake)
- [`log-logstash`](https://github.com/togo-framework/log-logstash) — Logstash log shipping for togo — streams JSON-line logs to a Logstash TCP input
- [`log-sentry`](https://github.com/togo-framework/log-sentry) — Sentry error tracking for togo — captures kernel error events with stack traces

## AI Kit

- **[`ai`](https://github.com/togo-framework/ai) — togo AI plugin — unified LLM interface (chat/embed/tools/stream) with a pluggable provider driver registry (openai, anthropic, gemini, ollama, …)**
- **[`rag-postgres`](https://github.com/togo-framework/rag-postgres) — PostgreSQL vector store for ai-rag — pgvector + pg_search BM25 hybrid retrieval**
- [`ai-adk`](https://github.com/togo-framework/ai-adk) — Google Agent Development Kit (ADK) integration for togo
- [`ai-agentops`](https://github.com/togo-framework/ai-agentops) — Agent operations & observability for togo — token/cost/latency tracking, feeds billing
- [`ai-agno`](https://github.com/togo-framework/ai-agno) — Agno agent framework integration for togo
- [`ai-anthropic`](https://github.com/togo-framework/ai-anthropic) — Anthropic Claude driver for togo ai
- [`ai-crawlee`](https://github.com/togo-framework/ai-crawlee) — Go-native site crawler data-source for the togo AI kit
- [`ai-deepseek`](https://github.com/togo-framework/ai-deepseek) — DeepSeek LLM driver for togo ai
- [`ai-firecrawl`](https://github.com/togo-framework/ai-firecrawl) — Firecrawl scrape/crawl data-source (self-hosted + API) for the togo AI kit
- [`ai-gemini`](https://github.com/togo-framework/ai-gemini) — Google Gemini driver for togo ai
- [`ai-grok`](https://github.com/togo-framework/ai-grok) — xAI Grok LLM driver for togo ai
- [`ai-ollama`](https://github.com/togo-framework/ai-ollama) — Ollama LLM driver for togo ai
- [`ai-openai`](https://github.com/togo-framework/ai-openai) — OpenAI LLM driver for togo ai
- [`ai-playwright`](https://github.com/togo-framework/ai-playwright) — Headless-browser (Playwright) data-source for the togo AI kit
- [`ai-qwen`](https://github.com/togo-framework/ai-qwen) — Qwen (DashScope) LLM driver for togo ai
- [`ai-rag`](https://github.com/togo-framework/ai-rag) — RAG capability for togo (on the ai plugin)
- [`ai-rss`](https://github.com/togo-framework/ai-rss) — RSS/Atom feed data-source for the togo AI kit
- [`ai-searxng`](https://github.com/togo-framework/ai-searxng) — SearXNG metasearch data-source for the togo AI kit
- [`ai-stt`](https://github.com/togo-framework/ai-stt) — Speech-to-Text for togo — Whisper + Deepgram drivers
- [`ai-tts`](https://github.com/togo-framework/ai-tts) — Text-to-Speech for togo — ElevenLabs + OpenAI TTS drivers (TTS_DRIVER)

## Payments & Billing

- **[`billing`](https://github.com/togo-framework/billing) — Usage-based billing + API keys for togo — per-user keys, AI token metering, quotas & usage reports**
- **[`payment`](https://github.com/togo-framework/payment) — togo payment subsystem — a Provider contract (charge/refund/checkout/customer/webhook) with a driver registry; Stripe, Paymob, Fawry, Tap, Moyasar, PayTabs, PayFort, Lemon Squeezy ship as driver plugins.**
- **[`subscriptions`](https://github.com/togo-framework/subscriptions) — Subscription management for togo — plans, trials, subscribe/cancel/change, over the payment plugin**
- [`payment-fawry`](https://github.com/togo-framework/payment-fawry) — Fawry driver for togo payment
- [`payment-lemonsqueezy`](https://github.com/togo-framework/payment-lemonsqueezy) — LemonSqueezy driver for togo payment
- [`payment-moyasar`](https://github.com/togo-framework/payment-moyasar) — Moyasar driver for togo payment
- [`payment-payfort`](https://github.com/togo-framework/payment-payfort) — PayFort driver for togo payment
- [`payment-paymob`](https://github.com/togo-framework/payment-paymob) — Paymob driver for togo payment
- [`payment-paytabs`](https://github.com/togo-framework/payment-paytabs) — PayTabs driver for togo payment
- [`payment-stripe`](https://github.com/togo-framework/payment-stripe) — Stripe driver for togo payment
- [`payment-tap`](https://github.com/togo-framework/payment-tap) — Tap driver for togo payment

## Deploy

- **[`deploy`](https://github.com/togo-framework/deploy) — togo deploy subsystem — provider-agnostic Deployer contract (provision/deploy/destroy) for clouds, VPS, Docker, Kubernetes & Terraform**
- [`deploy-aws`](https://github.com/togo-framework/deploy-aws) — AWS (App Runner) deploy driver for togo
- [`deploy-azure`](https://github.com/togo-framework/deploy-azure) — Azure (Container Apps) deploy driver for togo
- [`deploy-centos`](https://github.com/togo-framework/deploy-centos) — togo deploy driver: deploy-centos
- [`deploy-debian`](https://github.com/togo-framework/deploy-debian) — togo deploy driver: deploy-debian
- [`deploy-digitalocean`](https://github.com/togo-framework/deploy-digitalocean) — DigitalOcean deploy driver for togo
- [`deploy-docker`](https://github.com/togo-framework/deploy-docker) — togo deploy driver: deploy-docker
- [`deploy-gcp`](https://github.com/togo-framework/deploy-gcp) — Google Cloud (Cloud Run) deploy driver for togo
- [`deploy-hetzner`](https://github.com/togo-framework/deploy-hetzner) — Hetzner Cloud deploy driver for togo
- [`deploy-kubernetes`](https://github.com/togo-framework/deploy-kubernetes) — togo deploy driver: deploy-kubernetes
- [`deploy-ovh`](https://github.com/togo-framework/deploy-ovh) — OVHcloud (Public Cloud / OpenStack) deploy driver for togo
- [`deploy-terraform`](https://github.com/togo-framework/deploy-terraform) — togo deploy driver: deploy-terraform
- [`deploy-ubuntu`](https://github.com/togo-framework/deploy-ubuntu) — togo deploy driver: deploy-ubuntu
- [`deploy-vultr`](https://github.com/togo-framework/deploy-vultr) — Vultr deploy driver for togo

## DNS, Proxy & Gateway

- **[`dns`](https://github.com/togo-framework/dns) — togo DNS / reverse-proxy / API-gateway subsystem (base Provider contract)**
- [`dns-caddy`](https://github.com/togo-framework/dns-caddy) — Caddy reverse-proxy driver for the togo dns subsystem
- [`dns-cloudflare`](https://github.com/togo-framework/dns-cloudflare) — Cloudflare DNS driver for the togo dns subsystem
- [`dns-kong`](https://github.com/togo-framework/dns-kong) — Kong API-gateway driver (Supabase-friendly) for the togo dns subsystem
- [`dns-npm`](https://github.com/togo-framework/dns-npm) — Nginx Proxy Manager reverse-proxy driver for the togo dns subsystem

## Tunnels

- **[`tunnel`](https://github.com/togo-framework/tunnel) — togo public-tunnel subsystem — one contract over Cloudflare Tunnel, ngrok, Tailscale Funnel, frp**
- [`tunnel-cloudflare`](https://github.com/togo-framework/tunnel-cloudflare) — Cloudflare Tunnel driver for togo tunnel
- [`tunnel-frp`](https://github.com/togo-framework/tunnel-frp) — togo tunnel-frp plugin
- [`tunnel-ngrok`](https://github.com/togo-framework/tunnel-ngrok) — ngrok driver for togo tunnel (pure-Go SDK)
- [`tunnel-tailscale`](https://github.com/togo-framework/tunnel-tailscale) — togo tunnel-tailscale plugin

## Chat Bots

- **[`bot`](https://github.com/togo-framework/bot) — togo bot plugin**
- [`bot-discord`](https://github.com/togo-framework/bot-discord) — togo bot-discord plugin
- [`bot-slack`](https://github.com/togo-framework/bot-slack) — togo bot-slack plugin
- [`bot-telegram`](https://github.com/togo-framework/bot-telegram) — togo bot-telegram plugin

## i18n, Location & Settings

- **[`i18n`](https://github.com/togo-framework/i18n) — togo i18n provider plugin**
- **[`location`](https://github.com/togo-framework/location) — Localization dataset for togo — countries, currencies, dial codes, timezones, languages + lookup API**
- **[`settings`](https://github.com/togo-framework/settings) — Shared typed config store for togo — DB-backed, scoped, Go + REST API**
- **[`translation`](https://github.com/togo-framework/translation) — DB-backed dynamic i18n for togo — edit translations at runtime, falls back to the static i18n catalog**

## Multi-tenancy (SaaS)

- **[`saas`](https://github.com/togo-framework/saas) — Multi-tenant SaaS for togo: domain/tenant-id resolution + shared-DB or DB-per-tenant isolation**

## Documents

- **[`ocr`](https://github.com/togo-framework/ocr) — togo OCR plugin — image→text via tesseract (default) or the ai vision driver; POST /api/ocr**
- **[`pdf`](https://github.com/togo-framework/pdf) — togo HTML→PDF plugin — headless-Chromium driver, render API + POST /api/pdf**

## Contacts & CRM

- **[`contacts`](https://github.com/togo-framework/contacts) — togo contacts plugin**
- [`contacts-google`](https://github.com/togo-framework/contacts-google) — togo contacts-google plugin

## Dev & Testing

- **[`faker`](https://github.com/togo-framework/faker) — togo faker: fake data for factories/seeders**
- **[`testing`](https://github.com/togo-framework/testing) — togo test harness (HTTP + assertions + sqlite)**
- **[`validation`](https://github.com/togo-framework/validation) — togo request validation (Laravel-style rules)**
- [`testing-playwright`](https://github.com/togo-framework/testing-playwright) — togo plugin: testing-playwright

## Supabase

- **[`plugin-auth-supabase`](https://github.com/togo-framework/plugin-auth-supabase) — togo plugin: Supabase (GoTrue) JWT auth — /auth/me + bearer middleware**
- **[`supabase`](https://github.com/togo-framework/supabase) — togo Supabase integration: custom image (ParadeDB/pgvector/pg_partman) + stack**

## SEO

- **[`seo`](https://github.com/togo-framework/seo) — togo SEO/AEO plugin — sitemap, robots, llms.txt, meta/OG/JSON-LD + IndexNow / Google Analytics / Search Console / Bing providers.**

## Contributing

Built a togo plugin? **[Submit it to the marketplace](https://to-go.dev/marketplace/submit)** or open a PR. New plugins follow the [plugin-template](https://github.com/togo-framework/plugin-template) + the provider-driver pattern. This list is generated from the live togo-framework org.

## License

[MIT](LICENSE) © togo-framework.
