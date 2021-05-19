FROM node:alpine

WORKDIR '/usr/app'

COPY package.json .
Run npm install -g npm@7.13.0
RUN npm install
COPY . .

CMD ["npm","start"]
