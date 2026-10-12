# PetMatch — Evidencias de Sistema (Fase 2)

Avance de **PetMatch** para la fase 2 del ramo: frontend y backend al **~50%**. App para reportar mascotas perdidas, avistamientos y matching con apoyo de IA.

## Cómo correrlo

1. Copia las variables de entorno (las claves van solo en `.env`, **no se suben**):

```bash
copy .env.example .env
```

2. Completa en `.env` `DATABASE_URL`, `JWT_SECRET` y `GEMINI_API_KEY`.

3. Levanta el stack:

```bash
docker compose up --build
```

Por defecto la base es **Neon** (nube). Postgres local solo se inicia con:

```bash
docker compose --profile local-db up --build
```

## Puertos

- Frontend: http://localhost:3000
- Backend: http://localhost:8000
- pgAdmin: http://localhost:5050
