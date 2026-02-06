# techtest
test for developer jr
# Tech Test – Django + DRF + React + PostgreSQL

Proyecto de prueba con **backend en Django + Django REST Framework** y **frontend en React (Vite)** consumiendo una API REST.  
La base de datos es **PostgreSQL** (local via Docker). Incluye health check, CRUD de tareas, y soporte de filtros/búsqueda/orden.

---

## Stack
- Backend: Django, Django REST Framework
- DB: PostgreSQL
- Frontend: React + Vite
- CORS: django-cors-headers
- Infra local: Docker

---

## 1) PostgreSQL en Docker

Ejemplo (valores compatibles con `.env.example`):

```bash
docker run --name techtest-postgres \
  -e POSTGRES_DB=techtest \
  -e POSTGRES_USER=techtest_user \
  -e POSTGRES_PASSWORD=techtest_pass \
  -p 5432:5432 \
  -d postgres:16
