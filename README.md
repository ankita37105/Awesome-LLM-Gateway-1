# Awesome-LLM-Gateway

## Top LLM Gateway Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Unified LLM Routing, Load Balancing, Fallbacks, Caching, Cost Control, Guardrails & Observability*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **LLM Gateways** (AI Gateways). These systems provide a single OpenAI-compatible (or unified) API in front of many model providers, handling routing, retries, fallbacks, caching, rate limits, spend tracking, and often guardrails.



**Examples** include Portkey, OpenRouter, TrueFoundry AI Gateway, Kong AI Gateway, Azure AI Gateway, Cloudflare AI Gateway, Zuplo, Gravitee AI Gateway, Helicone, Braintrust, and LiteLLM Proxy (the category leaders).



**Open-source emphasis**: LLM gateways have excellent open options. **LiteLLM** is the most widely adopted self-hosted proxy; **Portkey Gateway** offers a strong open-source core with guardrails; Kong and others extend traditional API gateways. This section is heavily expanded with these tools.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saashosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

| Platform | Description / Key Features | Starting Paid Pricing | Free Tier / Free Trial Limits |
| :--- | :--- | :--- | :--- |
| **[Portkey](https://portkey.ai/)** | Production AI gateway with routing across 1,600+ models, deep observability, caching, fallbacks, and integrated guardrails. | **$49/month**<br>(Production tier: 100,000 recorded logs/mo included; +$9 per additional 100k requests) | **Free forever (Developer)**:<br>10,000 recorded logs/month, unlimited gateway proxy requests (requests are unblocked after cap, logs just stop recording), Universal API, playground & prompt management. |
| **[OpenRouter](https://openrouter.ai/)** | Hosted model aggregator and unified gateway providing OpenAI-compatible access to 200+ models with smart routing and analytics. | **$0.80 min fee / 5.5% platform fee** on card payments (5.0% on crypto); BYOK free for first 1M requests/mo then 5% platform fee; $0 token markup | **Free forever**:<br>50 requests/day (throttled at 20 req/min) across `:free` designated models (permanently increases to 1,000 requests/day after $10 lifetime credit purchase); 1M BYOK requests/month free. |
| **[TrueFoundry AI Gateway](https://www.truefoundry.com/)** | Enterprise AI gateway supporting cloud, VPC, on-prem, and air-gapped deployments with rate limits, spend controls, and RBAC governance. | **$499/month**<br>(Pro tier: 1,000,000 requests/mo, up to 10 user seats, predictability controls) | **Free forever (Developer)**:<br>50,000 requests/month, up to 3 user seats, playground & RBAC.<br>**7-day free trial** available for paid Pro tier. |
| **[Kong AI Gateway](https://konghq.com/)** | AI Gateway capabilities built into Kong Konnect, offering AI proxying, prompt routing, semantic caching, PII sanitization, and security plugins. | **$100/model/month + $200/million API requests**<br>(Konnect Plus modular tier; includes 1M base API requests/mo) | **30-day free trial** with full Enterprise functionality and unlimited gateway instances; plus free self-hosted open-source Kong Gateway core. |
| **[Cloudflare AI Gateway](https://www.cloudflare.com/)** | Edge-based AI gateway offering global response caching, rate limiting, analytics, and fallback routing across 300+ edge PoPs with zero added latency. | **$0 gateway fees**<br>(Optional **$5/month** Workers Paid plan expands log retention to 1,000,000 logs/mo and adds 10M Worker requests) | **Free forever**:<br>100,000 recorded logs/month across all gateways, unlimited gateway proxy requests (requests continue unblocked after log cap), 10,000 Neurons/day on Workers AI. |
| **[Zuplo](https://zuplo.com/)** | Serverless edge API management & AI gateway with native API key management, GitOps integration, and LLM rate limiting. | **$25/month**<br>(Builder tier: 2 custom domains, pay-as-you-go traffic scaling, custom branding) | **Free forever**:<br>100,000 requests/month, 2 gateway developers, unlimited API keys & environments, deployment to 300+ edge locations. |
| **[Gravitee AI Gateway](https://www.gravitee.io/)** | Enterprise API and AI management platform for policy enforcement, prompt security, LLM routing, and AI agent control planes. | **$2,500/month**<br>(Planet tier: 1 production gateway, unlimited API calls & events, gold enterprise support) | **14-day free trial** of enterprise cloud features with full gateway capabilities (no credit card required); plus free open-source Community Edition. |
| **[Azure API Management AI Gateway](https://azure.microsoft.com/)** | Managed cloud gateway with built-in AI policies for token rate limiting, semantic caching, and multi-endpoint load balancing across Azure OpenAI models. | **$3.50 per 1 million calls**<br>(Consumption tier pay-as-you-go) or **$48/month** (Developer / Basic dedicated instance) | **Free forever grant**:<br>1,000,000 API calls/month on Consumption tier;<br>**30-day free trial** with $200 Azure credits for new accounts. |
| **[Helicone](https://www.helicone.ai/)** | Developer-focused LLM gateway and observability platform offering smart caching, rate limiting, prompt evaluation, and auto-fallbacks. | **$79/month**<br>(Pro tier: 1,000 logs/min ingestion, 1-month data retention, alerts, unlimited seats) | **Free forever (Hobby)**:<br>10,000 requests/month, 10 logs/min ingestion, 1 GB storage, 7-day data retention, 1 seat. |
| **[Braintrust AI Proxy](https://www.braintrust.dev/)** | Hosted AI proxy and evaluation gateway unifying multiple LLM providers with automatic caching, prompt tracing, and dataset logging. | **$249/month**<br>(Pro tier: $100/mo model credits, 5 GB data, 50,000 scores/month, 30-day retention) | **Free forever (Starter)**:<br>$10/mo model credits, 1 GB/mo data, 10,000 scores/month, 14-day retention, unlimited seats; AI Proxy is free in public preview. |



## Open-Source GitHub Projects

- **[LiteLLM](https://github.com/BerriAI/litellm)**  

  Leading open-source LLM gateway and Python SDK (MIT) — call 100+ providers in OpenAI format, with proxy server, load balancing, fallbacks, cost tracking, virtual keys, and logging. The default self-hosted choice for many teams.



- **[Portkey Gateway](https://github.com/Portkey-AI/gateway)**  

  Open-source (MIT) AI gateway with routing, retries, caching, fallbacks, and integrated guardrails. Can be self-hosted; commercial cloud adds advanced observability and scale.



- **[Kong AI Gateway plugins / Kong Gateway](https://github.com/Kong/kong)**  

  Open-source API gateway with AI-specific plugins for LLM routing, rate limiting, and policy enforcement — ideal if you already run Kong.



- **[Open-source AI gateway experiments and forks](https://github.com/)**  

  Community projects that implement lightweight OpenAI-compatible proxies with routing and basic observability.



- **[Helicone (proxy mode)](https://github.com/Helicone/helicone)**  

  Open-source observability-focused proxy that can sit in front of LLM providers for logging and cost tracking.



- **[Custom OpenAI-compatible reverse proxies](https://github.com/)**  

  Lightweight open proxies built with FastAPI, Express, or Envoy that normalize provider APIs.



- **[RouteLLM and research routing frameworks](https://github.com/)**  

  Open routing logic that can be embedded into a self-hosted gateway for cost/quality-aware model selection.



- **[Virtual-key and budget-enforcement open modules](https://github.com/)**  

  Components that add team-level spend controls and key management on top of open gateways.



- **[Semantic caching open implementations](https://github.com/)**  

  Community caching layers often paired with LiteLLM or custom proxies to reduce cost and latency.



- **[OTEL-instrumented gateway sidecars](https://github.com/)**  

  Patterns that export gateway metrics and traces into existing open observability stacks.



### Additional Strong Open-Source Options

- Deploying **LiteLLM Proxy** when you want the broadest provider coverage and a battle-tested self-hosted gateway.

- Using **Portkey Gateway** when you also need built-in guardrails and a clean TypeScript/Node option.

- Extending **Kong** if your organization already standardizes on it for API management.

- Adding caching, virtual keys, and spend tracking on top of any open proxy.

- Accepting that fully managed multi-provider marketplaces (OpenRouter), edge global networks (Cloudflare), and deep enterprise governance still favor commercial/hosted platforms for some use cases.



**Frameworks for building custom systems**: Run LiteLLM or Portkey Gateway in your VPC → point all application traffic at the unified OpenAI-compatible endpoint → configure routing, fallbacks, and budgets → export logs and metrics to your observability stack. This gives full control and zero per-token markup. Commercial gateways (Portkey Cloud, OpenRouter, TrueFoundry, Kong Konnect, Cloudflare AI Gateway, etc.) remain attractive when you want managed scale, global edge presence, or turnkey multi-provider access without operating infrastructure.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- LLM gateways sit in the critical path of every model call and often handle API keys and potentially sensitive prompts. Secure the gateway itself (network isolation, authentication, audit logging, key rotation). Self-hosted deployments require proper high-availability, rate-limit, and monitoring configuration. Provider terms of service and data-processing agreements still apply to the underlying models. This list is not security or compliance advice.



---

**Made for platform engineers and AI teams who want one clean API in front of many models.**

Let's keep routing, cost control, and observability open and under your infrastructure.
