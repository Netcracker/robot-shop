FROM node:22-alpine

ENV INSTANA_AUTO_PROFILE true

EXPOSE 8080

WORKDIR /opt/server

COPY package*.json /opt/server/
COPY node_modules/ /opt/server/node_modules/

RUN npm install

COPY server.js /opt/server/

CMD ["node", "server.js"]

