# Base Image to build your image on
FROM node

# Run all commands in this container directory
WORKDIR /app

COPY package.json /app

# RUN - executed when creating an image
# Install all node dependencies
RUN npm install

# First (.) = soruce = Copy all files from where the Dockerfile currently lives 
# Second (.) = destination  = Store all files into the current working directory of the conatiner i.e /app
# COPY . .

# Another way of doing the above ^^
# Copy all code from nodejs_app into container /app folder
COPY . /app


# Expose port 80 to our local machine
EXPOSE 80

# CMD - Executed when a conatiner instance is started based on the image
# Once a container has been start -> execute command [node server.js]
CMD [ "node", "server.js" ]

