FROM node

WORKDIR /app

COPY . /app

COPY package.json /app

RUN npm install

EXPOSE 80

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

CMD [ "npm","start" ]

