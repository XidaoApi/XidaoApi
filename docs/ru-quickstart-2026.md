# XiDao AI API Gateway - Быстрый старт 2026

Единый API-шлюз для ведущих AI-моделей: Claude 4.7, GPT-5.5, Gemini 3.0 и других.
Совместимый с OpenAI API формат - просто меняйте `base_url`.

## Доступ

- Панель управления: https://global.xidao.online
- API Base URL: `https://api.global.xidao.online/v1`

## Установка

```bash
pip install openai httpx
```

## Получение API-ключа

1. Зарегистрируйтесь на https://global.xidao.online
2. Перейдите в раздел API Keys
3. Создайте новый ключ

## Пример 1: Базовый запрос (Python)

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ.get("XIDAO_API_KEY"),
    base_url="https://api.global.xidao.online/v1"
)

response = client.chat.completions.create(
    model="claude-4.7",
    messages=[
        {"role": "system", "content": "Ты полезный ассистент на русском языке."},
        {"role": "user", "content": "Объясни квантовые вычисления простыми словами."}
    ],
    temperature=0.7,
    max_tokens=1024
)

print(response.choices[0].message.content)
```

## Пример 2: Стриминг в реальном времени

```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.global.xidao.online/v1"
)

stream = client.chat.completions.create(
    model="gpt-5.5",
    messages=[
        {"role": "user", "content": "Напиши короткий рассказ о будущем AI в России"}
    ],
    stream=True,
    temperature=0.9
)

for chunk in stream:
    if chunk.choices[0].delta.content:
        print(chunk.choices[0].delta.content, end="", flush=True)
print()
```

## Пример 3: Переключение между моделями

```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.global.xidao.online/v1"
)

models = ["claude-4.7", "gpt-5.5", "gemini-3.0"]
prompt = "Что такое машинное обучение? Объясни в 3 предложениях."

for model in models:
    response = client.chat.completions.create(
        model=model,
        messages=[{"role": "user", "content": prompt}],
        max_tokens=200
    )
    print(f"\n=== {model} ===")
    print(response.choices[0].message.content)
```

## Пример 4: Автоматический Failover

```python
from openai import OpenAI

models_fallback = ["claude-4.7", "gpt-5.5", "gemini-3.0"]

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.global.xidao.online/v1"
)

def call_with_fallback(prompt, models):
    for model in models:
        try:
            response = client.chat.completions.create(
                model=model,
                messages=[{"role": "user", "content": prompt}],
                max_tokens=500
            )
            print(f"Успех с моделью: {model}")
            return response.choices[0].message.content
        except Exception as e:
            print(f"Ошибка с {model}: {e}")
            continue
    return "Все модели недоступны"

result = call_with_fallback("Привет, как дела?", models_fallback)
print(result)
```

## Пример 5: Работа с Embeddings

```python
from openai import OpenAI

client = OpenAI(
    api_key="your-xidao-api-key",
    base_url="https://api.global.xidao.online/v1"
)

response = client.embeddings.create(
    model="text-embedding-3-large",
    input=["Привет мир", "Машинное обучение", "Искусственный интеллект"]
)

for i, embedding in enumerate(response.data):
    print(f"Текст {i+1}: размерность {len(embedding.embedding)}")
    print(f"  Первые 5 значений: {embedding.embedding[:5]}")
```

## Доступные модели (2026)

| Модель | ID модели | Лучший вариант для |
|--------|-----------|---------------------|
| Claude 4.7 | `claude-4.7` | Анализ, рассуждение, безопасность |
| Claude 4.7 Sonnet | `claude-4.7-sonnet` | Быстрые ответы, код |
| GPT-5.5 | `gpt-5.5` | Универсальные задачи |
| GPT-5.5 Turbo | `gpt-5.5-turbo` | Низкая задержка, массовые запросы |
| Gemini 3.0 Pro | `gemini-3.0-pro` | Мультимодальные задачи |
| Gemini 3.0 Flash | `gemini-3.0-flash` | Скорость, стоимость |

## Полезные ссылки

- Панель: https://global.xidao.online
- Документация API: https://global.xidao.online/docs
- Статус сервиса: https://global.xidao.online/status

## FAQ

**В: Какие библиотеки поддерживаются?**
О: Любая библиотека, совместимая с OpenAI API (openai, httpx, langchain, llama-index и др.)

**В: Есть ли бесплатный пробный период?**
О: Да, зарегистрируйтесь на https://global.xidao.online для получения бесплатных кредитов.

**В: Поддерживается ли русский язык?**
О: Да, все модели отлично работают с русскоязычными запросами.

---

*Создано XiDao AI API Gateway - 2026*
