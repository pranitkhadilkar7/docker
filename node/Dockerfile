FROM node
WORKDIR /node-app
COPY package.json /node-app
RUN yarn
COPY . /node-app
EXPOSE 3000
CMD [ "node", "server.js" ]