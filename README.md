# Essence Backend

## // About

A secure, modern messaging backend inspired by Signal, but without the need for phone numbers. It will feature end-to-end encryption, real-time notifications, Spotify presence integration. Purely built with Rust with a workspace-based architecture.

## // Workspace Structure Overview

### This is still a work in progress.

- **astral** — Cryptography helpers (E2EE, Key Management,...)
- **aurora** — WS Server
- **echo** — Shared models & DTOs
- **eden** — Authentication & Indentity
- **january** — RESTful API
- **lumen** — Background daemon for tasks
- **starlight** — Core utilities
- **solstice** — Database
- **sonar** — Integrations & Connections

## // Services

| Service     | Description             | URL / Port             |
| ----------- | ----------------------- | ---------------------- |
| Postgres    | Relational DB           | localhost:5432         |
| MongoDB     | NoSQL Document DB       | localhost:27017        |
| Redis       | In-memory datastore     | localhost:6379         |
| RabbitMQ    | Message broker (AMQP)   | localhost:5672         |
| RabbitMQ UI | RabbitMQ Management UI  | http://localhost:15672 |
| MinIO       | Object storage          | http://localhost:9001  |
| MailDev     | SMTP & webmail dev tool | http://localhost:1080  |
| Keycloak    | Identity & Auth server  | http://localhost:8082  |
| Nginx       | Reverse proxy / gateway | http://localhost       |
