# Telegram Bot (Python)

Proyecto minimo para un bot de Telegram con polling usando python-telegram-bot.

## Requisitos
- Docker
- Token en `TELEGRAM_BOT_TOKEN`

## Configuracion
1) Copia el archivo de entorno:

```bash
cp .env.example .env
```

2) Edita `.env` y agrega tu token.

## Desarrollo (hot reload)
Desde la raiz del repo:

```bash
docker compose up --build
```

## Produccion
Desde la raiz del repo:

```bash
docker build -t telegram-bot .
docker run --env-file .env telegram-bot
```
