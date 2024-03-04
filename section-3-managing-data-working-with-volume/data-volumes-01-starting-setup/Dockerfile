FROM node
WORKDIR /app
COPY package.json .
RUN yarn
COPY . .
EXPOSE 80
CMD [ "node", "server.js" ]