# frontend/Dockerfile
FROM nginx:latest

# Копіюємо конфігураційний файл Nginx
COPY nginx.conf /etc/nginx/nginx.conf

# Копіюємо статичні файли у відповідну папку Nginx
COPY templates /usr/share/nginx/html

# Виставляємо порт
EXPOSE 8000