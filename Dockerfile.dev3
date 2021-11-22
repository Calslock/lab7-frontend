FROM node:alpine

WORKDIR '/app'
ENV NODE_OPTIONS=--openssl-legacy-provider
COPY package.json .
RUN npm install

RUN chown -R node:node /app

CMD ["npm", "run", "start"]