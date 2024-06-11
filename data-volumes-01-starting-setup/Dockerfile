FROM node:12

WORKDIR /apps

COPY package.json /apps

RUN npm install

COPY . /apps

ARG DEFAULT_PORT=80

ENV PORT ${DEFAULT_PORT}

EXPOSE $PORT

# VOLUME [ "/apps/node_modules" ]

CMD [ "npm", "start" ]