# Awesome-LLM-Gateway

## Top LLM Gateway Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Unified LLM Routing, Load Balancing, Fallbacks, Caching, Cost Control, Guardrails & Observability*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **LLM Gateways** (AI Gateways). These systems provide a single OpenAI-compatible (or unified) API in front of many model providers, handling routing, retries, fallbacks, caching, rate limits, spend tracking, and often guardrails.



**Examples** include Portkey, OpenRouter, TrueFoundry AI Gateway, Kong AI Gateway, Azure AI Gateway, Cloudflare AI Gateway, Zuplo, Gravitee AI Gateway, FuseAI Gateway, and LiteLLM Proxy (the category leaders).



**Open-source emphasis**: LLM gateways have excellent open options. **LiteLLM** is the most widely adopted self-hosted proxy; **Portkey Gateway** offers a strong open-source core with guardrails; Kong and others extend traditional API gateways. This section is heavily expanded with these tools.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Portkey](https://portkey.ai/)**  

  Production AI gateway with routing across 1,600+ models, deep observability, caching, fallbacks, and integrated guardrails (open-source gateway core + managed cloud).



- **[OpenRouter](https://openrouter.ai/)**  

  Hosted aggregator/marketplace providing one API key and unified access to hundreds of models from many providers with routing and usage analytics.



- **[TrueFoundry AI Gateway](https://www.truefoundry.com/)**  

  Enterprise AI gateway with strong support for VPC, on-prem, and air-gapped deployments plus governance features.



- **[Kong AI Gateway](https://konghq.com/)**  

  AI-specific capabilities layered on Kong’s mature API gateway platform — routing, plugins, and policy control for LLM traffic.



- **[Azure AI Gateway / Azure AI services](https://azure.microsoft.com/)**  

  Microsoft’s managed gateway and routing options within the Azure AI / Foundry ecosystem.



- **[Cloudflare AI Gateway](https://www.cloudflare.com/)**  

  Edge-based AI gateway offering caching, analytics, and simple routing with a generous free tier.



- **[Zuplo](https://zuplo.com/)**  

  API gateway platform with AI/LLM-focused features for developers and teams.



- **[Gravitee AI Gateway](https://www.gravitee.io/)**  

  API management platform extended with AI gateway capabilities for enterprise control planes.



- **[FuseAI Gateway and similar offerings](https://github.com/)**  

  Additional commercial AI gateways focused on unified access, security, and observability.



- **[Other managed LLM / AI gateways](https://github.com/)**  

  Cloud-provider and specialist gateways that consolidate model access behind a single endpoint.



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
