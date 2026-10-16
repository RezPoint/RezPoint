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

## Избранные проекты

### [deskly-crm](https://github.com/RezPoint/deskly-crm)
Лёгкая CRM для малого бизнеса: клиенты, заказы, товары, задачи и платежи. **Go + GORM + SQLite** на backend, **React + TypeScript** на frontend. Разделение данных пользователей через JWT; собранный SPA раздаётся одним бинарником.

**Другие открытые репозитории:**

- [prolongation-analysis](https://github.com/RezPoint/prolongation-analysis) — анализ пролонгаций.
- [diagnostic_system](https://github.com/RezPoint/diagnostic_system) — диагностическая система.
- [todolist](https://github.com/RezPoint/todolist) — менеджер задач.
- [txt-to-json-converter](https://github.com/RezPoint/txt-to-json-converter) — конвертация текстовых данных в JSON.

## Open Source

### [Twenty CRM](https://github.com/twentyhq/twenty) — диагностика ошибки авторизации

**[Issue #27255](https://github.com/twentyhq/twenty/issues/27255)** · **[Fix PR #27318](https://github.com/twentyhq/twenty/pull/27318)** · `High priority · Fixed`

Обнаружил и описал ошибку: защищённые HTTP-маршруты Logic Functions возвращали **500 Internal Server Error** при отсутствии авторизации вместо корректной ошибки доступа.

- Подготовил воспроизводимый баг-репорт с шагами и окружением.
- Исследовал исходный код и указал на возможную причину — обработку `AuthException` в фильтре исключений.
- Проблему подтвердили, присвоили высокий приоритет и **исправили в принятом PR #27318**.

*Мой вклад — обнаружение, диагностика и репорт ошибки; код исправления написан другим участником.*

## Непубличные проекты

Часть рабочих и личных проектов находится в закрытых репозиториях:

- **avito-scanner** — Telegram-бот для мониторинга объявлений: aiogram, Playwright, httpx, управление прокси, фоновые asyncio-задачи, кластеризация через scikit-learn.
- **finance-tracker** — десктопный учёт финансов: мультивалютные счета, операции, долги и криптоактивы; Electron, React, SQLite WASM.

## Контакты

- **Сайт:** [anstanta.dev](https://anstanta.dev)
- **Email:** [rezpoin@gmail.com](mailto:rezpoin@gmail.com)
- **GitHub:** [@RezPoint](https://github.com/RezPoint)
