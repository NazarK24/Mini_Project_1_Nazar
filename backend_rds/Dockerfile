# backend_rds/Dockerfile
FROM python:3.9-slim

WORKDIR /app

# Копіюємо файли проекту
COPY backend_rds/backend_rds /app/backend_rds
COPY backend_rds/core /app/core
COPY backend_rds/requirements.txt /app

# Встановлюємо залежності
RUN pip install --no-cache-dir -r requirements.txt

# Вказуємо порт для сервера
EXPOSE 8000

# Запускаємо сервер
CMD ["python", "core/manage.py", "runserver", "0.0.0.0:8000"]