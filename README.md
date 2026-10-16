<div align="center">

# Привет, я Артём 👋

**Backend Developer · Python / Go · API & Automation**

Разрабатываю backend-сервисы, инструменты автоматизации и приложения — от идеи и архитектуры до развёртывания.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

</div>

---

## Обо мне

Основной фокус — **Python backend**: асинхронная обработка данных, интеграции с внешними API, базы данных и сервисы автоматизации. Также разрабатываю на **Go** и **TypeScript**, работаю с Linux-инфраструктурой. Изучаю **C++** и системное программирование.

Люблю разбираться не только в том, *как* работает код, но и в том, *почему* он ведёт себя именно так.

## Технологии

| Направление | Инструменты |
| --- | --- |
| **Backend** | Python 3.11+, asyncio, FastAPI, aiohttp, httpx, asyncpg, Go (net/http, GORM) |
| **Данные** | PostgreSQL, SQLite |
| **Автоматизация** | aiogram, Playwright |
| **Frontend & Desktop** | TypeScript, React, Vite, Electron |
| **Инфраструктура** | Linux, Docker, systemd, GitHub Actions, Amvera, structlog |

## Избранные публичные проекты

### [DesklyCRM](https://github.com/RezPoint/deskly-crm) · Go / React / SQLite

CRM для малого бизнеса: клиенты, заказы, товары, задачи, частичные оплаты и дашборд. **Go (net/http, GORM)** для API, **React + TypeScript** для интерфейса, SQLite для хранения данных; JWT-авторизация и разделение данных по tenant. Приложение собирается в один серверный бинарник со встроенным SPA.

### [TodoList — Telegram Bot & Mini App](https://github.com/RezPoint/todolist) · TypeScript / Fastify / React

Монорепозиторий системы управления задачами: **Telegram-бот, Mini App и общий REST API**. Backend на Fastify + Prisma, интерфейс на React + Tailwind CSS, бот на grammY; общие данные, валидация Zod и Swagger-документация.

### [unbake-test — Audio Alignment R&D](https://github.com/RezPoint/unbake-test) · Python / ASR / ML

Исследовательский прототип для получения текста песен с **таймкодами отдельных слов**. Сравнение faster-whisper и выравнивания через wav2vec2-CTC + `torchaudio.forced_align`; метрики качества, замеры производительности и воспроизводимые эксперименты в Colab. Результаты и ограничения описаны в design doc.

**Другие проекты с открытым кодом:**

- **[tg-userbot](https://github.com/RezPoint/tg-userbot)** — мониторинг Telegram-каналов с фриланс-заказами: Telethon, фильтрация лидов, SQLite и уведомления.
- **[diagnostic_system](https://github.com/RezPoint/diagnostic_system)** — десктопная диагностика ПК: Python, PyQt5, мониторинг аппаратных ресурсов и PDF-отчёты.
- **[prolongation-analysis](https://github.com/RezPoint/prolongation-analysis)** — анализ пролонгаций договоров: pandas, расчёт коэффициентов и генерация Excel-отчётов.
- **[txt-to-json-converter](https://github.com/RezPoint/txt-to-json-converter)** — утилита преобразования вложенных текстовых категорий в JSON.

## Open Source

### [Twenty CRM](https://github.com/twentyhq/twenty) — диагностика ошибки авторизации

**[Issue #27255](https://github.com/twentyhq/twenty/issues/27255)** · **[Fix PR #27318](https://github.com/twentyhq/twenty/pull/27318)** · `High priority · Fixed`

Обнаружил и описал ошибку: защищённые HTTP-маршруты Logic Functions возвращали **500 Internal Server Error** при отсутствии авторизации вместо корректной ошибки доступа.

- Подготовил воспроизводимый баг-репорт с шагами и окружением.
- Исследовал исходный код и указал на возможную причину — обработку `AuthException` в фильтре исключений.
- Проблему подтвердили, присвоили высокий приоритет и **исправили в принятом PR #27318**.

*Мой вклад — обнаружение, диагностика и репорт ошибки; код исправления написан другим участником.*


### [Hermes Agent](https://github.com/NousResearch/hermes-agent) — совместимость Python-зависимостей

**[Issue #133254](https://github.com/NousResearch/hermes-agent/issues/133254)** · **[Fix PR #134305](https://github.com/NousResearch/hermes-agent/pull/134305)** · `P2 · Fix proposed`

Обнаружил и воспроизвёл проблему обновления зависимостей Hermes Agent: при `hermes pm update --uv` разрешение зависимостей приводило к попытке собрать устаревший `spaCy 2.0.17` под **Python 3.14**, из-за чего обновление завершалось ошибкой.

- Описал точные шаги воспроизведения, окружение Linux и проблемную цепочку `kittentts → spaCy`.
- Другой участник воспроизвёл проблему на macOS и установил первопричину в работе `uv` с override-зависимостью.
- Подготовлено исправление с регрессионными тестами; **PR #134305 открыт и ожидает рассмотрения**.

*Мой вклад — обнаружение и документирование ошибки. Анализ первопричины и код исправления — @kokhlo; PR открыл @liuhao1024.*

## Непубличные проекты

Часть проектов и рабочих решений находится в закрытых репозиториях. Ниже — описание задач и используемых технологий без публикации исходного кода.

- **Маркетплейс-аналитика (Wildberries / Ozon)** — асинхронные Python-сервисы для сбора рекламной и аналитической статистики через API, обработки данных в PostgreSQL и формирования Excel-отчётов. `asyncio`, `aiohttp`, `asyncpg`, `openpyxl`, Telegram-интеграции.
- **avito-scanner** — мониторинг объявлений с ценовыми порогами, дедупликацией, семантической фильтрацией и уведомлениями в Telegram. Python, aiogram, Playwright, httpx, SQLite.
- **finance-tracker** — локальное десктоп-приложение для мультивалютного учёта финансов и криптоактивов. Electron, React, SQLite WASM, Bybit API.
- **shorts-factory (экспериментальный)** — конвейер обработки AI-новостей и генерации коротких видео: LLM, TTS, субтитры, ffmpeg, интеграция с YouTube; Python и Docker.

## Контакты

- **Сайт:** [anstanta.dev](https://anstanta.dev)
- **Email:** [rezpoin@gmail.com](mailto:rezpoin@gmail.com)
- **GitHub:** [@RezPoint](https://github.com/RezPoint)
