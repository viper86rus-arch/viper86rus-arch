# ⚡ V1PER (`viper86rus-arch`)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg?logo=python&logoColor=white)](https://www.python.org/)
[![Architecture](https://img.shields.io/badge/Architecture-Asyncio_%26_Event_Loop-orange.svg)]()
[![Standard](https://img.shields.io/badge/Policy-Zero_Bloat_%2F_Zero_Pip-blueviolet.svg)]()
[![Code Quality](https://img.shields.io/badge/Quality-PEP8_%26_Type_Hints-009688.svg)]()
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> **Инженерная разработка прикладных систем и бэкенда на Python.**  
> Специализируюсь на асинхронных конвейерах, обратной разработке закрытых API маркетплейсов, отказоустойчивых Telegram-платформах и сетевых утилитах.  
> Фокус: максимальная производительность, предсказуемость под нагрузкой и минимальный оверхед внешних зависимостей.

---

## 🛠 Инженерные принципы в коде

* **Приоритет Standard Library (Zero-Bloat):** если задачу можно эффективно решить средствами встроенных библиотек Python (`asyncio`, `urllib`, `socket`, `sqlite3`, `dataclasses`), я не подключаю десятки сторонних pip-пакетов. Это гарантирует мгновенный запуск и отсутствие конфликта версий.
* **Асинхронная устойчивость:** проектирование сетевых систем с жёстким контролем параллелизма через `asyncio.Semaphore`, строгими таймаутами соединений и защитой от исчерпания файловых дескрипторов ОС.
* **Честная доставка данных:** экспорт таблиц в строгом стандарте Excel (`UTF-8 BOM`, русские разделители `;`), валидация структур и транзакционная запись без блокировок.
* **Производственная культура:** все модули содержат чистую обработку системных сигналов (`SIGINT` / Ctrl+C, exit code 130), подробное логирование и автономные `--demo` режимы для сквозного тестирования без внешней сети.

---

## 📁 Флагманские проекты (Showcase)

| Проект | Стек | Решённая инженерная задача |
|---|---|---|
| 🎯 **[Wildberries_Fast_Scraper](https://github.com/viper86rus-arch/Wildberries_Fast_Scraper)** | Python 3, Direct HTTP API, Zero-Pip | Высокоскоростной парсер каталога WB. Автокалькуляция цен со скидками СПП (WB Кошелёк), складская аналитика по РФ, экспорт в Excel/JSON, фильтрация и демо-режим. |
| ⚡ **[Async_TCP_Scanner](https://github.com/viper86rus-arch/Async_TCP_Scanner)** | Python 3, `asyncio`, Socket API, Zero-Pip | Асинхронный сканер TCP-портов на Single-Thread Event Loop. Двухфазный захват баннеров служб (SSH/HTTP), контроль дескрипторов семафором, экспорт с таймингами. |
| 🌐 **[Enterprise_Web_Scraper](https://github.com/viper86rus-arch/Enterprise_Web_Scraper)** | Python 3, Playwright, FastAPI, SQLite | Парсинг динамических страниц в Stealth-режиме с блокировкой медиа-трафика. Web UI Dashboard для операторов, неблокирующий запуск и стриминг логов по WebSockets. |
| 🤖 **[Telegram_Commercial_Bot](https://github.com/viper86rus-arch/Telegram_Commercial_Bot)** | Python 3, Telegram Bot API, ReportLab | Платформа продаж под ключ. Интерактивный расчёт смет, векторный генератор A4 PDF со штампом цифровой подписи (63-ФЗ), эквайринг, микро-CRM на SQLite. |

---

## 💻 Технический стек

* **Язык и ядро:** Python 3.9 – 3.12 (`asyncio`, `multiprocessing`, `threading`, `dataclasses`, `typing`).
* **Парсинг и сетевой I/O:** Reverse-Engineering мобильных/внутренних API, Playwright, HTTP/SOCKS5 проксирование с авторизацией, эмуляция отпечатков (Anti-Detect).
* **Базы данных и экспорт:** SQLite3 (неблокирующий пул через потоки), PostgreSQL, OpenPyXL, CSV `UTF-8-SIG`.
* **Интерфейсы и интеграции:** Telegram Bot API (Long Polling, Telegram Payments, Custom UI), FastAPI, REST API, генерация документов PDF (ReportLab / низкоуровневый PDF Stream).
* **Среды развёртывания:** Linux (Ubuntu, Debian, RHEL), macOS, Windows Server.

---

## 📄 Лицензия и авторство

* **Автор разработки:** V1PER ([`viper86rus-arch`](https://github.com/viper86rus-arch))
* **Лицензия:** [MIT License](LICENSE) (2026) — открытый исходный код без ограничений на коммерческое и образовательное применение.
