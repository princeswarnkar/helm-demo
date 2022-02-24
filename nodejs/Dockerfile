FROM node:14-alpine3.14
WORKDIR /work
COPY package.json .
RUN npm install
COPY . .
ENTRYPOINT [ "npm","start" ]
