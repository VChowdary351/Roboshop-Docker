FROM node:14-alpine
EXPOSE 8080
WORKDIR /opt/server
ENV MONGO=true
COPY package.json .
COPY server.js .
RUN npm install
CMD [ "node", "server.js" ]