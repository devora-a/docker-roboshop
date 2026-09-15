FROM node:20
# this creats /app and move there
WORKDIR /app
COPY package.json .
COPY *.JS .
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node", "server.js"]
