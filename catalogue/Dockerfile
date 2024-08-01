FROM node:18.19.1-alpine3.19
EXPOSE 8080
RUN addgroup -S roboshop && adduser -S roboshop -G roboshop 
WORKDIR /opt/server
ENV MONGO=true
USER roboshop
COPY package.json .
COPY server.js .
RUN npm install -g npm@10.8.2
RUN npm install --silent
CMD [ "node", "server.js" ]