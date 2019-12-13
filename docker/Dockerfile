FROM node:10
WORKDIR /usr/src/app
COPY ../package*.json ./
RUN npm install
RUN npm install --global mocha
RUN npm install request --save
COPY ../. .
RUN chmod +x ./script/test.sh
EXPOSE 8080
CMD [ "node", "index.js" ]
