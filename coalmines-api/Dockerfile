FROM node:10

WORKDIR /usr/src/app

COPY app/build/bundle/package*.json ./
RUN npm install --production
COPY app/build/bundle/src ./

EXPOSE 3000

CMD [ "node", "." ]
