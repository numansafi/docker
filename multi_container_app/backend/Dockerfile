FROM node

WORKDIR /app

COPY . /app

COPY package.json /app

RUN npm install

EXPOSE 80

CMD [ "node","app.js" ]

