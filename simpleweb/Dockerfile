# Use an existing docker image as a base
FROM node:alpine

# Setting up WORKDIR
WORKDIR /usr/app

# copy file to WORKDIR
COPY ./package.json ./
# Download and install a dependency
RUN npm install

# Separate copy actions to minimize cache busting and rebuild
COPY ./ ./

#EXPOSE
EXPOSE TCP/8080

# Tell the image what to do when it starts as a container
CMD ["npm", "start"]
