     1|# XiDao API Gateway
     2|
     3|[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
     4|[![Website](https://img.shields.io/website?url=https%3A%2F%2Fxidaoapi.com&label=Website)](https://xidaoapi.com)
     5|[![OpenAI Compatible](https://img.shields.io/badge/OpenAI-Compatible-blue.svg)](https://xidaoapi.com)
     6|[![Models](https://img.shields.io/badge/Models-100%2B-green.svg)](https://xidaoapi.com)
     7|
     8|Affordable OpenAI-compatible AI API gateway for developers and startups.
     9|
    10|Access 100+ LLM models through a single API endpoint - Claude, GPT, Gemini, DeepSeek, Mistral, Qwen, and more.
    11|
    12|---
    13|
    14|## Quick Start
    15|
    16|```python
    17|from openai import OpenAI
    18|
    19|client = OpenAI(
    20|    api_key="your-xidao-api-key",
    21|    base_url="https://api.xidaoapi.com/v1"
    22|)
    23|
    24|response = client.chat.completions.create(
    25|    model="claude-4.7",
    26|    messages=[{"role": "user", "content": "Hello!"}]
    27|)
    28|print(response.choices[0].message.content)
    29|```
    30|
    31|## Open-Source Tools and Examples
    32|
    33|| Repository | Description |
    34||------------|-------------|
    35|| [agent-eval-toolkit](https://github.com/XidaoApi/agent-eval-toolkit) | Evaluate LLM agent outputs across providers — tool-use validation, regression testing, cost-aware scoring |
    36|| [xidao-python-examples](https://github.com/XidaoApi/xidao-python-examples) | Python SDK examples - chat, streaming, embeddings, multi-provider switching |
    37|| [xidao-nodejs-examples](https://github.com/XidaoApi/xidao-nodejs-examples) | Node.js/TypeScript - streaming, Vercel AI SDK, endpoint migration |
    38|| [xidao-cookbook](https://github.com/XidaoApi/xidao-cookbook) | Migration guides, failover patterns, cost control recipes |
    39|| [llm-api-bench](https://github.com/XidaoApi/llm-api-bench) | Benchmark LLM providers on latency, throughput, cost, and quality |
    40|| [llm-cost-calculator](https://github.com/XidaoApi/llm-cost-calculator) | Compare pricing across 50+ providers and estimate monthly costs |
    41|| [llm-failover-router-demo](https://github.com/XidaoApi/llm-failover-router-demo) | Production failover router with circuit breakers and health checks |
    42|| [mcp-server-template](https://github.com/XidaoApi/mcp-server-template) | MCP server template with multi-provider routing and observability |
    43|| [llm-provider-migration-checklist](https://github.com/XidaoApi/llm-provider-migration-checklist) | Safe provider switching checklist with regression test suite |
    44|| [llm-output-checker-action](https://github.com/XidaoApi/llm-output-checker-action) | GitHub Action to validate LLM responses in CI/CD pipelines |
    45|| [llm-prompt-tester](https://github.com/XidaoApi/llm-prompt-tester) | Test and compare LLM prompts across providers - quality scoring, latency, cost |
    46|
    47|## Why Developers Choose XiDao
    48|
    49|- **Drop-in compatible** - Works with OpenAI SDK, just change `base_url`
    50|- **100+ models** - Claude 4.7, GPT-5.5, Gemini 3.0 Pro, DeepSeek V4, Qwen 3, Mistral Large, and more
    51|- **Smart routing** - Automatic failover between providers with circuit breakers
    52|- **Cost optimization** - Route to cheaper models for simple tasks, premium for complex ones
    53|- **MCP support** - Model Context Protocol tools for AI agent integrations
    54|- **Free $10 credit** - Start testing immediately, no credit card required
    55|
    56|## Links
    57|
    58|- Website: https://xidaoapi.com
    59|- Support: support@xidao.online
    60|- Telegram: https://t.me/ccyu085
    61|
    62|---
    63|
    64|## Russian
    65|
    66|XiDao AI API Gateway - edinyy API-shlyuz dlya dostupa k vedushchim AI-modelyam 2026 goda.
    67|
    68|**Dostupnye modeli:** Claude 4.7, GPT-5.5, Gemini 3.0 Pro, DeepSeek V4, Qwen 3, Mistral Large i drugie.
    69|
    70|**Preimushchestva:**
    71|- Sovmestimost' s OpenAI API - prosto menyayte `base_url`
    72|- Intellektual'nyy routing i avtomaticheskiy failover
    73|- Optimizatsiya stoimosti cherez marshrutizatsiyu
    74|- Podderzhka MCP dlya AI-agentov
    75|- Besplatnyy kredit $10 dlya novykh pol'zovateley
    76|
    77|**Bysrtyy start:**
    78|```python
    79|from openai import OpenAI
    80|
    81|client = OpenAI(
    82|    api_key="your-xidao-api-key",
    83|    base_url="https://api.xidaoapi.com/v1"
    84|)
    85|
    86|response = client.chat.completions.create(
    87|    model="claude-4.7",
    88|    messages=[{"role": "user", "content": "Privet!"}]
    89|)
    90|print(response.choices[0].message.content)
    91|```
    92|
    93|**Poleznye ssylki:**
    94|- Sayt: https://xidaoapi.com
    95|- Python primery: [xidao-python-examples](https://github.com/XidaoApi/xidao-python-examples)
    96|- Node.js primery: [xidao-nodejs-examples](https://github.com/XidaoApi/xidao-nodejs-examples)
    97|- Cookbook: [xidao-cookbook](https://github.com/XidaoApi/xidao-cookbook)
    98|
    99|---
   100|*Last updated: 2026-05-14*
   101|