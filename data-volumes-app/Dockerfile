FROM node

WORKDIR /app

COPY package.json /app

RUN npm install

COPY . /app

EXPOSE 80

# Dir path inside the container which should be mapped to 
# folder outside the container i.e on the host machine
# where data will survive, even if the conatiner has been stopped or removed
# CREATES AN ANONYMOUS VOLUME
VOLUME [ "/app/feedback" ]

CMD [ "npm", "start" ]

