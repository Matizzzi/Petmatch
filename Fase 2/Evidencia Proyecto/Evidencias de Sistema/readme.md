# PetMatch — Evidencias de Sistema (Fase 2)

Frontend (Expo) y backend (FastAPI) de PetMatch: reportes de mascotas perdidas, avistamientos, matching heurístico y análisis de fotos con IA.

## Seguridad

Las claves **no van en GitHub**. Copia la plantilla y completa tus valores locales:

```bash
copy .env.example .env
```

En `.env` define al menos:

- `DATABASE_URL`
- `JWT_SECRET`
- `GROQ_API_KEY` (opcional, para Analizar con IA; plan Free en https://console.groq.com/keys)

`GEMINI_API_KEY` es opcional. Si no hay ninguna clave de visión, el backend usa un análisis local de pelaje.

## Cómo correrlo

1. Instala Docker Desktop.
2. En esta carpeta: `copy .env.example .env` y completa las variables.
3. En Windows puedes usar `iniciar.bat`, o en terminal:

```bash
docker compose up --build
```

Postgres local (opcional):

```bash
docker compose --profile local-db up --build
```

## Puertos

| Servicio | URL |
| :--- | :--- |
| Frontend | http://localhost:3000 |
| Backend / Swagger | http://localhost:8000/docs |
| pgAdmin | http://localhost:5050 |

pgAdmin local: `admin@petmatch.com` / `admin` (solo desarrollo).
