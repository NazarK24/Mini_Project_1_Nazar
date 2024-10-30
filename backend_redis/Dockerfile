# backend_redis/Dockerfile
FROM python:3.9-slim

WORKDIR /app

# Копіюємо файли проекту
COPY backend_redis/backend_redis /app/backend_redis
COPY backend_redis/core /app/core
COPY backend_redis/requirements.txt /app

# Встановлюємо залежності
RUN pip install --no-cache-dir -r requirements.txt

# Вказуємо порт для сервера
EXPOSE 8001

# Запускаємо сервер
CMD ["python", "core/manage.py", "runserver", "0.0.0.0:8001"]