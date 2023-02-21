# Use nodejs as a base image
FROM node:14

# Container Working directory
WORKDIR /app

COPY package.json /app

RUN npm install 

# Copy all other files into container /app dir
COPY . /app

EXPOSE 3000

# Execute Node command
CMD [ "node", "app.mjs" ]