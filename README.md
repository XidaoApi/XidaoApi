# XiDao API Gateway

🚀 Affordable OpenAI-compatible AI API gateway for developers and startups.

Access 100+ LLM models through a single API endpoint — Claude, GPT, Gemini, DeepSeek, Mistral, Qwen, and more.

## Quick Start

```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.global.xidao.online/v1"
)

response = client.chat.completions.create(
    model="claude-4.7",
    messages=[{"role": "user", "content": "Hello!"}]
)
print(response.choices[0].message.content)
```

## Open-Source Tools & Examples

| Repository | Description |
|------------|-------------|
| [xidao-python-examples](https://github.com/XidaoApi/xidao-python-examples) | Python SDK examples — chat, streaming, embeddings, multi-provider switching |
| [xidao-nodejs-examples](https://github.com/XidaoApi/xidao-nodejs-examples) | Node.js/TypeScript — streaming, Vercel AI SDK, endpoint migration |
| [xidao-cookbook](https://github.com/XidaoApi/xidao-cookbook) | Migration guides, failover patterns, cost control recipes |
| [llm-api-bench](https://github.com/XidaoApi/llm-api-bench) | Benchmark LLM providers on latency, throughput, cost, and quality |
| [llm-cost-calculator](https://github.com/XidaoApi/llm-cost-calculator) | Compare pricing across 50+ providers and estimate monthly costs |
| [llm-failover-router-demo](https://github.com/XidaoApi/llm-failover-router-demo) | Production failover router with circuit breakers and health checks |
| [mcp-server-template](https://github.com/XidaoApi/mcp-server-template) | MCP server template with multi-provider routing and observability |
| [llm-provider-migration-checklist](https://github.com/XidaoApi/llm-provider-migration-checklist) | Safe provider switching checklist with regression test suite |
| [llm-output-checker-action](https://github.com/XidaoApi/llm-output-checker-action) | GitHub Action to validate LLM responses in CI/CD pipelines |

## Why Developers Choose XiDao

- **Drop-in compatible** — Works with OpenAI SDK, just change `base_url`
- **100+ models** — Claude 4.7, GPT-5.5, Gemini 3.0 Pro, DeepSeek V4, Qwen 3, Mistral Large, and more
- **Smart routing** — Automatic failover between providers with circuit breakers
- **Cost optimization** — Route to cheaper models for simple tasks, premium for complex ones
- **MCP support** — Model Context Protocol tools for AI agent integrations
- **Free $10 credit** — Start testing immediately, no credit card required

## Links

- 🌐 Website: https://global.xidao.online/
- 📧 Support: support@xidao.online
- 💬 Telegram: https://t.me/ccyu085

## Русский язык / Russian

XiDao AI API Gateway — единый API-шлюз для доступа к ведущим AI-моделям 2026 года.

**Доступные модели:** Claude 4.7, GPT-5.5, Gemini 3.0 Pro, DeepSeek V4, Qwen 3, Mistral Large и другие.

**Преимущества:**
- Совместимость с OpenAI API — просто меняйте `base_url`
- Интеллектуальный роутинг и автоматический failover
- Оптимизация стоимости через маршрутизацию
- Поддержка MCP для AI-агентов
- Бесплатный кредит $10 для новых пользователей

**Быстрый старт:**
```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.global.xidao.online/v1"
)

response = client.chat.completions.create(
    model="claude-4.7",
    messages=[{"role": "user", "content": "Привет!"}]
)
print(response.choices[0].message.content)
```

**Полезные ссылки:**
- 🌐 Сайт: https://global.xidao.online/
- 🐍 Python примеры: [xidao-python-examples](https://github.com/XidaoApi/xidao-python-examples)
- 📦 Node.js примеры: [xidao-nodejs-examples](https://github.com/XidaoApi/xidao-nodejs-examples)
- 📚 Cookbook: [xidao-cookbook](https://github.com/XidaoApi/xidao-cookbook)
