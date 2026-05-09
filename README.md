# Django + React Server Setup

Автоматический bootstrap-скрипт для быстрого поднятия сервера под Django + React проекты на Ubuntu/Debian.

Устанавливает:
- Nginx
- Python 3
- pip
- Git
- Node.js
- npm
- Yarn
- Certbot
- python3-certbot-nginx
- curl

Подходит для:
- Django
- Django REST Framework
- React / Vue / Nuxt фронтенда
- Fullstack deployment
- VPS bootstrap
- Быстрой подготовки сервера под прод

---

# Быстрый запуск

```bash
curl -fsSL bit.ly/reactdjango | bash
```

---

# Что делает скрипт

## Обновляет систему

```bash
apt update && apt upgrade -y
```

## Устанавливает базовые пакеты

```bash
nginx
python3
python3-pip
git
nodejs
npm
curl
```

## Устанавливает Yarn

Добавляет официальный репозиторий Yarn и устанавливает пакет.

## Устанавливает SSL инструменты

```bash
certbot
python3-certbot-nginx
```

Позволяет быстро подключить HTTPS через Let's Encrypt.

---

# Требования

- Ubuntu / Debian
- Root доступ
- Свежий VPS

---

# Проверка установки

## Python

```bash
python3 --version
```

## Node.js

```bash
node -v
```

## Yarn

```bash
yarn -v
```

## Nginx

```bash
systemctl status nginx
```

---

# Пример получения SSL

```bash
certbot --nginx -d example.com -d www.example.com
```

---

# Безопасность

Перед запуском рекомендуется проверить содержимое скрипта:

```bash
curl -fsSL bit.ly/reactdjango
```

Не запускай неизвестные install-скрипты без проверки.

---

# Roadmap

Планируемое:
- Docker
- Docker Compose
- PostgreSQL
- Redis
- UFW setup
- Fail2Ban
- Gunicorn
- PM2
- Авто-конфиг Nginx
- CI/CD helpers

---

# License

MIT

---

# Автор

GitHub: https://github.com/danilax9
