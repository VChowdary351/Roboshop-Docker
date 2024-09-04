FROM nginx
RUN rm -rf /usr/share/nginx/html/index.html&&rm -rf /etc/nginx/nginx.conf&&rm -rf /etc/nginx/conf.d/default.conf
COPY roboshop.conf /etc/nginx/nginx.conf
EXPOSE 80
ADD static /usr/share/nginx/html/