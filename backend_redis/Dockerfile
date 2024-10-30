FROM python:3.11-slim

WORKDIR /app

COPY . .

RUN pip install --no-cache-dir -r requirements.txt

ENV DJANGO_SETTINGS_MODULE=backend_redis.settings

EXPOSE 8001

CMD ["python", "manage.py", "runserver", "0.0.0.0:8001"]