FROM node:lts

WORKDIR /app

COPY ./app/package.json ./

RUN npm install -g npm@latest

RUN yarn install

COPY ./app ./

EXPOSE 5173

CMD ["yarn", "dev", "--host"]