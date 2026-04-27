# Артём

Python-разработчик. Делаю асинхронные сервисы сбора и анализа данных, ботов, небольшие веб- и десктопные приложения.

## Стек

**Основной:** Python 3.11+, asyncio, aiohttp/httpx, asyncpg, PostgreSQL, SQLite, FastAPI, aiogram, Playwright

**Параллельно использую:** Go (GORM, net/http), TypeScript, React, Vite, Electron

**Инфраструктура:** Docker, systemd, Amvera, GitHub Actions, structlog

## Публичные проекты

- **[deskly-crm](https://github.com/RezPoint/deskly-crm)** — лёгкая CRM для малого бизнеса: клиенты, заказы, товары, задачи, платежи. Бэкенд на Go + GORM + SQLite, фронтенд на React + TypeScript, multi-tenant через JWT. Один бинарник раздаёт собранный SPA.
- **[prolongation-analysis](https://github.com/RezPoint/prolongation-analysis)** — анализ пролонгаций.
- **[diagnostic_system](https://github.com/RezPoint/diagnostic_system)** — диагностическая система.
- **[todolist](https://github.com/RezPoint/todolist)** — приложение для управления задачами.
- **[txt-to-json-converter](https://github.com/RezPoint/txt-to-json-converter)** — утилита конвертации.

## Закрытые проекты

Код не публикую, ниже короткое описание стека и решённых задач.

- **avito-scanner** — Telegram-бот для мониторинга новых объявлений на Авито. aiogram + Playwright (stealth) + httpx, прокси-менеджер с blacklist'ом, фоновые задачи на asyncio с self-restarting loop, кластеризация через scikit-learn.
- **finance-tracker** — десктопное приложение для учёта личных финансов: счета в разных валютах, доходы/расходы/переводы, долги, криптопортфель с подтягиванием балансов из Bybit. Electron + React + node-sqlite3-wasm.

## Связь

- Email: rezpoin@gmail.com
- GitHub: [@RezPoint](https://github.com/RezPoint)
