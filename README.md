# Радиф Илалтдинов

**Senior Backend / Full Stack разработчик. Автоматизирую процессы. Внедряю ИИ.**

Python (FastAPI, Django, AsyncIO) · TypeScript (React) · PostgreSQL · Redis · Docker · GitLab CI/CD ·
локальные LLM, RAG, мульти-агентные системы.

Казань · удалённо, гибридно, готов к переезду · 7+ лет в коммерческой разработке, стаж подтверждён
электронной трудовой книжкой.

**[Резюме — radif.ru](https://radif.ru)** · [Демо ИИ-агента](https://radif.ru/#demo) ·
[Telegram @radif_ru](https://t.me/radif_ru) · [i@radif.ru](mailto:i@radif.ru) ·
[Habr Career](https://career.habr.com/radif-ru)

## Сейчас

- **Старший разработчик и системный аналитик** в ООО «Творческое Образование» — две штатные
  должности с 2025 года. Платформа для двух федеральных сетей школ (GRAFIKA и ArtTech): веб,
  Android, iOS и Telegram-бот на одной кодовой базе. С 2026 года отвечаю за backend, frontend,
  DevOps, QA, архитектуру и системную аналитику.
- **Магистратура НИЯУ МИФИ**, 2026–2028 — «Обработка данных и применение искусственного
  интеллекта», очная форма. Параллельно зачислен на Цифровую кафедру МИФИ (программа федерального проекта «Университеты для поколения лидеров») — второй диплом о профессиональной переподготовке, программа
  «Вайб-кодинг: разработка приложений с помощью AI».

## Цифры, которые можно проверить

| Число      | Что                                                                                       | Где проверить                                                                                      |
| ---------- | ----------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **889**    | unit-тестов во флагманском проекте, покрытие 88% при гейте ≥80%                           | [tests](https://github.com/radif-ru/ai-multi-agent-system/tree/main/tests)                         |
| **7**      | автоматических гейтов качества в CI — все детерминированные, без ИИ                       | [test.yml](https://github.com/radif-ru/ai-multi-agent-system/blob/main/.github/workflows/test.yml) |
| **≈5 000** | студентов заведено в продакшн федеральной платформы моими скриптами загрузки и миграции   | [radif.ru/#platform-launch](https://radif.ru/#platform-launch)                                     |
| **2**      | федеральные сети школ на одной кодовой базе                                               | [radif.ru/#one-codebase](https://radif.ru/#one-codebase)                                           |
| **240+**   | задач и 20+ спринтов за четыре месяца на моей схеме ИИ-ассистированной разработки         | [radif.ru/#ai-process](https://radif.ru/#ai-process)                                               |
| **13**     | ИТ-компетенций подтверждено независимой оценкой Минцифры, все на продвинутом уровне       | [radif.ru/#certificates-mincifry](https://radif.ru/#certificates-mincifry)                         |
| **0**      | обращений к облачным LLM-API: инференс, эмбеддинги, vision и дообучение — на своём железе | [radif.ru/#hardware](https://radif.ru/#hardware)                                                   |

## Открытые проекты

- **[ai-multi-agent-system](https://github.com/radif-ru/ai-multi-agent-system)** — флагман.
  Локальная мульти-агентная система на self-hosted LLM (Ollama): цикл thought → action →
  observation, роли Planner / Executor / Critic, 19 инструментов (почта, Яндекс.Диск, веб, OCR,
  cron-планировщик), три канала — Telegram, MAX и консоль — на одном доменном контракте,
  RAG-память на sqlite-vec, vision и голос. 15 спринтов с Definition of Ready / Done,
  observability в self-hosted GlitchTip. [Скриншоты живых сессий](https://radif.ru/#demo).
- **[local-rag-mcp](https://github.com/radif-ru/local-rag-mcp)** — локальная база знаний на RAG
  и MCP: гибридный поиск BM25 + векторный со слиянием RRF, cross-encoder reranker, FAISS, ответы
  локальной LLM через Ollama.
- **[fine-tuning](https://github.com/radif-ru/fine-tuning)** — дообучение LLM методом LoRA (PEFT)
  на моделях из HuggingFace Hub.
- **[www](https://github.com/radif-ru/www)** — исходный код radif.ru: без фреймворков и сборки,
  0 рантайм-зависимостей, Docker + Nginx на своём VPS, строгий CSP, 7 проверок в CI.

Ранние проекты — в основном 2021 года и раньше: Django, DRF + React, PyQt, data mining, свой
веб-фреймворк — лежат в [списке репозиториев](https://github.com/radif-ru?tab=repositories);
часть демо до сих пор работает на моём VPS.

## Как я работаю

- **Детерминированное — скриптом, а не ИИ.** Линтеры, тесты, контроль покрытия, синхронность
  документации и деплойные проверки — гейты в CI и один `preflight` до коммита. ИИ остаётся там,
  где нужно суждение.
- **ИИ-агенты ускоряют рутину, но не решают за инженера.** Один свод правил `AGENTS.md` для
  Cursor, Windsurf, Devin, Claude Code, GitHub Copilot и JetBrains AI; архитектура, ревью и
  финальные решения — за мной.
- **Проверяю результат, а не намерение.** После деплоя скрипт сверяет статусы всех джобов
  пайплайна и доступность стендов: «задеплоил» не означает «надеюсь, доехало».
- **Разбираюсь, как устроено под капотом.** С фреймворками читаю исходники, а часть инструментов
  писал сам: свой веб-фреймворк, клиент-сервер на голых сокетах.

## Рабочий проект — масштаб без деталей под NDA

45+ таблиц PostgreSQL · ~100 версионных миграций · 140+ REST-эндпоинтов · 35+ тыс. строк бэкенда ·
110+ тыс. строк фронтенда · 9 ролей пользователей · 200+ unit-тестов на бэкенде и 140+ на
фронтенде, сквозные сценарии на Playwright · GitLab CI: у бэкенда 9 стадий и 22 джоба, у
фронтенда 8 стадий и 20 джобов, по три контура — тестовый стенд и два прода. Подробно —
[radif.ru/#job-creative](https://radif.ru/#job-creative).

## Стек

- **Backend:** Python, FastAPI, Django, Django REST framework, AsyncIO, SQLAlchemy 2.0 async,
  asyncpg, Alembic, Pydantic, Celery, Socket.IO, WebSocket, REST, GraphQL
- **Frontend:** TypeScript, JavaScript, React, Vue.js, Vite, Feature-Sliced Design, Effector,
  Vitest, Playwright, Storybook
- **Данные и брокеры:** PostgreSQL, Redis, SQLite, MySQL, MongoDB, RabbitMQ, MQTT
- **DevOps:** Linux, Docker, Docker Compose, Nginx, GitLab CI/CD, GitHub Actions, Let's Encrypt,
  Zabbix
- **ИИ:** Ollama, мульти-агентные системы, RAG, sqlite-vec, FAISS, MCP, LoRA fine-tuning,
  Tesseract OCR, faster-whisper, vision-модели

<details>
<summary>In English</summary>

Senior Backend / Full Stack engineer, 7+ years in commercial development (edtech, fintech,
vending, telephony). Python (FastAPI, Django, AsyncIO), TypeScript (React), PostgreSQL, Docker,
GitLab CI/CD. I build local-first AI: multi-agent systems on self-hosted LLMs, RAG, MCP,
fine-tuning. Master's student at MEPhI (data processing and AI, 2026–2028). Full resume in
Russian: [radif.ru](https://radif.ru).

</details>
