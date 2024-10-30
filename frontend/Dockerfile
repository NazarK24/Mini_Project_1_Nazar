FROM nginx:latest

COPY config.json /usr/share/nginx/html/config.json

COPY templates /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]