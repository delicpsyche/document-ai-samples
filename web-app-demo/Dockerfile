FROM node:20-slim

ENV APP_HOME /app
WORKDIR $APP_HOME

COPY . ./

# hadolint ignore=DL3000
WORKDIR ./Frontend

RUN npm install && npm run build

EXPOSE 8081

CMD [ "node", "server.js" ]
