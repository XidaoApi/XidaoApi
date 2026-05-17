# XiDao API Gateway

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Website](https://img.shields.io/website?url=https%3A%2F%2Fxidaoapi.com&label=Website)](https://xidaoapi.com)
[![OpenAI Compatible](https://img.shields.io/badge/OpenAI-Compatible-blue.svg)](https://xidaoapi.com)
[![Models](https://img.shields.io/badge/Models-100%2B-green.svg)](https://xidaoapi.com)

The affordable OpenAI-compatible AI API gateway for developers, startups, and AI agents.

Access 100+ LLM models through a single API endpoint — Claude, GPT, Gemini, DeepSeek, Qwen, Mistral, Llama, and more. Smart routing, automatic failover, and cost optimization built in.

---

## Quick Start

```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.xidaoapi.com/v1"
)

response = client.chat.completions.create(
    model="claude-4.7",
    messages=[{"role": "user", "content": "Hello!"}]
)
print(response.choices[0].message.content)
```

## Open-Source Tools and Examples

| Repository | Description |
|------------|-------------|
| [agent-eval-toolkit](https://github.com/XidaoApi/agent-eval-toolkit) | Evaluate LLM agent outputs across providers — tool-use validation, regression testing, cost-aware scoring |
| [local-llm-router](https://github.com/XidaoApi/local-llm-router) | Route prompts between local and cloud LLMs by task complexity — save 80%+ on AI costs |
| [xidao-python-examples](https://github.com/XidaoApi/xidao-python-examples) | Python SDK examples — chat, streaming, embeddings, multi-provider switching |
| [xidao-nodejs-examples](https://github.com/XidaoApi/xidao-nodejs-examples) | Node.js/TypeScript — streaming, Vercel AI SDK, endpoint migration |
| [xidao-cookbook](https://github.com/XidaoApi/xidao-cookbook) | Migration guides, failover patterns, cost control recipes |
| [llm-api-bench](https://github.com/XidaoApi/llm-api-bench) | Benchmark LLM providers on latency, throughput, cost, and quality |
| [llm-cost-calculator](https://github.com/XidaoApi/llm-cost-calculator) | Compare pricing across 50+ providers and estimate monthly costs |
| [llm-failover-router-demo](https://github.com/XidaoApi/llm-failover-router-demo) | Production failover router with circuit breakers and health checks |
| [mcp-server-template](https://github.com/XidaoApi/mcp-server-template) | MCP server template with multi-provider routing and observability |
| [llm-provider-migration-checklist](https://github.com/XidaoApi/llm-provider-migration-checklist) | Safe provider switching checklist with regression test suite |
| [llm-output-checker-action](https://github.com/XidaoApi/llm-output-checker-action) | GitHub Action to validate LLM responses in CI/CD pipelines |
| [llm-prompt-tester](https://github.com/XidaoApi/llm-prompt-tester) | Test and compare LLM prompts across providers — quality scoring, latency, cost |

## Why Developers Choose XiDao

- **Drop-in compatible** — Works with OpenAI SDK, just change `base_url`
- **100+ models** — Claude 4.7, GPT-5.5, Gemini 3.0 Pro, DeepSeek V4, Qwen 3, Mistral Large, Llama 4, and more
- **Smart routing** — Automatic failover between providers with circuit breakers
- **Cost optimization** — Route to cheaper models for simple tasks, premium for complex ones
- **MCP support** — Model Context Protocol tools for AI agent integrations
- **Free $10 credit** — Start testing immediately, no credit card required

## Links

- Website: https://xidaoapi.com
- Support: support@xidao.online
- Telegram: https://t.me/ccyu085

---

## Russian

XiDao AI API Gateway — edinyy API-shlyuz dlya dostupa k vedushchim AI-modelyam 2026 goda.

**Dostupnye modeli:** Claude 4.7, GPT-5.5, Gemini 3.0 Pro, DeepSeek V4, Qwen 3, Mistral Large, Llama 4 i drugie.

**Preimushchestva:**
- Sovmestimost' s OpenAI API — prosto menyayte `base_url`
- Intellektual'nyy routing i avtomaticheskiy failover
- Optimizatsiya stoimosti cherez marshrutizatsiyu
- Podderzhka MCP dlya AI-agentov
- Besplatnyy kredit $10 dlya novykh pol'zovateley

**Bysrtyy start:**
```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.xidaoapi.com/v1"
)

response = client.chat.completions.create(
    model="claude-4.7",
    messages=[{"role": "user", "content": "Privet!"}]
)
print(response.choices[0].message.content)
```

**Poleznye ssylki:**
- Sayt: https://xidaoapi.com
- Python primery: [xidao-python-examples](https://github.com/XidaoApi/xidao-python-examples)
- Node.js primery: [xidao-nodejs-examples](https://github.com/XidaoApi/xidao-nodejs-examples)
- Cookbook: [xidao-cookbook](https://github.com/XidaoApi/xidao-cookbook)

---
*Last updated: 2026-05-17*
