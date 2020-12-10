FROM nginx:1.9

COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./nginx/files/localhost.crt /etc/ssl/certs/nginx/localhost.crt
COPY ./nginx/files/localhost.key /etc/ssl/certs/nginx/localhost.key

EXPOSE 80
EXPOSE 443

CMD ["nginx", "-g", "daemon off;"]