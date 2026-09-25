# Sergey Kolomiichuk

Go backend developer. 10 years in industrial automation (SCADA, PLC) before moving to software.

I work on backends where the interesting part is not the handler: asynchronous processing
through queues, integration with external APIs that fail, media storage, rate limiting,
and knowing what the service does when a dependency is down.

`Go` `PostgreSQL` `Redis` `NATS JetStream` `MinIO` `gRPC` `REST API` `Docker` `Prometheus` `Grafana` `GitHub Actions`

## Work

**[Linka](https://github.com/Linka-masterskaya/zip-backend)** — commercial REST API + AI worker.
Text-to-speech generation runs through a NATS JetStream queue with an audio bank that
deduplicates repeated phrases; media lives in MinIO, rate limiting is done in Redis with
Lua scripts. I also set up the deployment pipeline and review code.

**[Yandex.Razvitie](https://github.com/yandex-development-1-team/go)** — REST API + Telegram bot,
Jan — Apr 2026. Backend for a corporate bot: service booking and request tracking,
Yandex.Forms webhook integration, files in MinIO, JWT auth. Layered architecture,
integration tests on Testcontainers, metrics in Prometheus.

## Projects

**[tamper](https://github.com/SergeyKo17/tamper)** — gRPC fault-injection proxy.
Sits between services and injects faults into live traffic: failures and data corruption,
at call level and at single messages inside a stream. It knows no protobuf schemas — it
relays a call as a bidirectional stream and works with message bytes, so it attaches to
any service without code generation. YAML config with hot reload, TLS on both sides.

**[jot](https://github.com/SergeyKo17/jot)** — MCP memory server for AI agents.
Four tools, one binary, zero config.

## Writing

About Go on Habr, in Russian:
[metrics and tracing](https://habr.com/ru/articles/1024854/) ·
[a public mock interview at Yandex](https://habr.com/ru/articles/1059542/) ·
[leading a team of juniors](https://habr.com/ru/articles/1001706/)

Telegram channel about Go — conclusions from real tasks and what to watch for
in implementation.

[![Telegram](https://img.shields.io/badge/Telegram-prod--logs-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/prodlogs)

## Contacts

Telegram: [@SergeyEn123](https://t.me/SergeyEn123)  
Email: sr.kolomiichuk@yandex.com


[![LeetCode Stats](https://leetcard.jacoblin.cool/s_kolomiichuk)](https://leetcode.com/s_kolomiichuk)
