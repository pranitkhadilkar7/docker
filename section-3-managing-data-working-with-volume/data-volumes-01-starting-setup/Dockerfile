FROM node
WORKDIR /app
COPY package.json .
RUN yarn
COPY . .
ENV PORT 80
EXPOSE $PORT
CMD [ "node", "server.js" ]