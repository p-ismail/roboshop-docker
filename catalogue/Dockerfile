FROM node:20
#this create /app and move to the directory
WORKDIR /app
COPY package.json .
COPY server.js .
RUN npm install
ENV MONGO="true" \
    MONGO_URL= "mongodb://mongo:27017/catalogue"

CMD ["node","server.js"]