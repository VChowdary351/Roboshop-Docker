FROM node:16-alpine
EXPOSE 8080
RUN addgroup -S roboshop && adduser -S roboshop -G roboshop 
WORKDIR /opt/server
ENV MONGO=true
USER roboshop
COPY package.json .
COPY server.js .
RUN npm install
CMD [ "node", "server.js" ]