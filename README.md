# XiDao API

Affordable OpenAI-compatible AI API gateway for developers and startups.

## What we build
- OpenAI-compatible endpoint for faster migration
- Multi-model access for GPT, Claude, Gemini, and more
- Lower-cost routing path for AI products and automation workflows
- Practical examples and migration guides for engineering teams

## Start here
- [XiDao Python Examples](https://github.com/XidaoApi/xidao-python-examples) — Chat, streaming, embeddings, multi-provider switching
- [XiDao Node.js Examples](https://github.com/XidaoApi/xidao-nodejs-examples) — Streaming, Vercel AI SDK, endpoint migration
- [XiDao Cookbook](https://github.com/XidaoApi/xidao-cookbook) — Migration guides, failover patterns, cost control
- [LLM Failover Router Demo](https://github.com/XidaoApi/llm-failover-router-demo) — Production failover with circuit breakers
- [LLM Cost Calculator](https://github.com/XidaoApi/llm-cost-calculator) — Compare pricing across 50+ providers
- [MCP Server Template](https://github.com/XidaoApi/mcp-server-template) — Build MCP servers with multi-provider routing
- [LLM Provider Migration Checklist](https://github.com/XidaoApi/llm-provider-migration-checklist) — Safe switching between providers
- [LLM Output Checker Action](https://github.com/XidaoApi/llm-output-checker-action) — Validate LLM responses in CI/CD
- Website: https://global.xidao.online/

## Why developers use XiDao
- switch from OpenAI-compatible SDK flows with minimal code changes
- test lower-cost model options without rebuilding app logic
- use practical migration and rollout guides before production traffic moves

## Contact
- Support: support@xidao.online
- Telegram: https://t.me/ccyu085

## Русский язык / Russian

Добро пожаловать! XiDao AI API Gateway — это единый API-шлюз для доступа к ведущим AI-моделям 2026 года.

**Доступные модели:** Claude 4.7, GPT-5.5, Gemini 3.0 Pro и другие.

**Преимущества:**
- Совместимость с OpenAI API — просто меняйте `base_url`
- Низкие цены через интеллектуальный роутинг
- Автоматический failover между моделями
- Поддержка русского языка во всех моделях

**Быстрый старт:**
```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.global.xidao.online/v1"
)

response = client.chat.completions.create(
    model="claude-4.7",
    messages=[{"role": "user", "content": "Привет! Расскажи о себе."}]
)
print(response.choices[0].message.content)
```

**Полезные ссылки:**
- Сайт: https://global.xidao.online
- Python примеры: [xidao-python-examples](https://github.com/XidaoApi/xidao-python-examples)
- Node.js примеры: [xidao-nodejs-examples](https://github.com/XidaoApi/xidao-nodejs-examples)